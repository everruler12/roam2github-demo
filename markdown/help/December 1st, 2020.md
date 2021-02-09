- [[sci]]
    - single block namespace
        - ```clojure
(ns my-stuff
  (:require
   [reagent.core :as r]))

(defn counter [_]
  (let [*count (r/atom 1)]
    (fn [_]
      [:button
       {:draggable true
        :on-click (fn [evt] (swap! *count inc))}
       @*count])))```
        - {{roam/cljs-render: ((CQNCL76xL))}}
    - multi block namespace (reference file)
        - {{roam/cljs-render: ((leFTj1Tvl))}}
        - code/my file
            - ```clojure
(ns my-stuff
  (:require
   [reagent.core :as r]))```
            - ```clojure
(defn counter [_]
  (let [*count (r/atom 11)]
    (fn [_]
      [:button
       {:on-click (fn [evt] (swap! *count inc))}
       @*count])))```
    - multi block namespace (reference single fn)
        - {{roam/cljs-render: ((PVrJu_Y8S))}}
        - code/my file
            - ```clojure
(ns my-stuff
  (:require
   [reagent.core :as r]))```
            - ```clojure
(defn my-inc [n]
  (* n 2))```
            - ```clojure
(defn counter2 [_]
  (let [*count (r/atom 2)]
    (fn [_]
      [:button
       {:on-click (fn [evt] (swap! *count my-inc))}
       @*count])))```
            - ```clojure
(defn counter [_]
  (let [*count (r/atom 0)]
    (fn [_]
      [:button
       {:on-click (fn [evt] (swap! *count inc))}
       @*count])))```
    - js window
        - {{roam/cljs-render: ((UdliV2uud))}}
        - ```clojure
(defn my-comp [_]
  [:div (pr-str (.. js/Number -MAX_VALUE))])```
    - datascript reactive
        - {{roam/cljs-render: ((yj2HtwWYh)) a b c}}
        - ```clojure
(ns async-stuff
  (:require
   [datascript.core :as d]
   [roam.datascript.reactive :as dr]))

(defn test [{:keys [block-uid]} & args]
  (let [*b (dr/f-entity d/touch [:block/uid block-uid])]
    (js/console.log args)
    (fn [& args]
      [:div "helo"
        (pr-str @*b)
		(with-out-str (prn @*b))])))
```
        - Example 2
            - ```clojure
;; Me me me
(ns example2
  (:require
   [datascript.core :as d]
   [roam.datascript.reactive :as dr]))
```
            - ```clojure

(def color ["#2EE115" "rgb(0,244,255)" "#F44336"])
```
            - ```clojure
(defn all-descendents-as-cards [block-entity]
[:div 
        (doall (for [block (rest (tree-seq :block/uid :block/children block-entity))]
          [:button.bp3-card
           	{:style {:background-color (rand-nth color)}
             :on-click (fn [e] (js/alert (:block/uid block)))}
           (:block/string block)]))
		]
)```
            - ```clojure

(defn test [{:keys [block-uid]} & args]
  (let [*my-children (dr/pull '[{:block/children ...} 
                      :block/string 
                      :block/uid] 
                              [:block/uid block-uid])]
    (js/console.log args)
    (fn [& args]
      [:div 
        (doall (for [block (rest (tree-seq :block/uid :block/children @*my-children))]
          [:button.bp3-card
           	{:style {:background-color (rand-nth color)}
             :on-click (fn [e] (js/alert (:block/uid block)))}
           (:block/string block)]))
		])))

(defn test2 [{:keys [block-uid]} & args]
  (let [*my-children (dr/pull '[{:block/_refs ...}
                                {:block/children ...} 
                      :block/string 
                      :block/uid] 
                      [:node/title "TODO"])]
    (js/console.log args)
    (fn [& args]
      [:div 
        (doall (for [block (rest (tree-seq :block/uid :block/_refs @*my-children))]
          [:button.bp3-card.green
           	{:style {:background-color (rand-nth color)}
             :on-click (fn [e] (js/alert (:block/uid block)))}
           (:block/string block)]))
		])))```
            - {{roam/render: ((qz-VHQwBC))}}
                - Block
                    - A
                    - B
                    - C
                - Me
                    - me
                    - me 
                        - me
            - {{[[TODO]]}} [[TODO]] this one
                - a
                - b
            - 
    - print lines
        - {{roam/cljs-render: ((2Xwl-F2aT))}}
        - ```clojure

(println "asdf")
(pr "asdf")
(prn "asdf")
(print "asdf")

(ns my-stuff
  (:require
   [clojure.pprint :as pp]))

(defn test-prints
  [{:keys [block-uid]}]
  (pp/pprint block-uid)
  (println "asdf")
  (pr "asdf")
  (prn "asdf")
  (print "asdf")
  [:div "test print"])```
    - Summary of what you need to know
        - {{[[TODO]]}} Put this at the top of your file
            - Code
                - ```clojure
(ns starting-point-for-custom-roam
  (:require
   [reagent.core :as r]
   [datascript.core :as d]
   [roam.datascript.reactive :as dr]))```
                - ```clojure
(defn *page-with-children-by-node-title [name] 
  	(dr/pull '[{:block/children ...}
               :block/string 
               :block/uid 
               :block/props
              ]
             [:node/title name])
  )```
                - ```clojure
(defn block-with-children-by-uid [name] 
  	(dr/pull '[
               {:block/children ...}
               {:block/path ...}
               :block/string 
               :block/uid 
               :block/props
              ]
             [:block/uid name])
  )```
                - ```clojure

(defn all-children [ent]
  	(:block/children ent)
  )

(defn controlled-input [my-local-string]
   [:div 
              "My local string is controlled by the input" 
              [:li  @my-local-string]
              
             [:input {:value @my-local-string
                      :on-change 
                      (fn [event] 
                        (reset! my-local-string 
                             (.. event -target -value)))}]
             
             ]
  )

(declare color)

(defn counter [my-local-number]
               [:div "I have been clicked"
             [:button {:on-click 
                       (fn [e] (swap! my-local-number inc))}
               @my-local-number]
              " times"]
  )
```
                - ```clojure

(def color ["#2EE115" "rgb(0,244,255)" "#F44336"])
``` [*](((oYL_2lm6B)))
                -  
                - ```clojure
(defn all-descendents-as-cards [block-entity]
[:div 
    (doall (for [block (rest (tree-seq :block/uid :block/children block-entity))]
          [:button.bp3-card
           	{:style {:background-color (rand-nth color)}
             :on-click (fn [e] (js/alert (:block/uid block)))}
           (:block/string block)]))
		]
)``` [*](((Fv9oJp3HV)))
                - ```clojure


(defn test [{:keys [block-uid]} & args]
  (let [*my-children (dr/pull '[{:block/children ...} 
                      :block/string 
                      :block/uid] 
                              [:block/uid block-uid])]
    (js/console.log args)
    (fn [& args]
      [:div 
        (doall (for [block (rest (tree-seq :block/uid :block/children @*my-children))]
          [:button.bp3-card
           	{:style {:background-color (rand-nth color)}
             :on-click (fn [e] (js/alert (:block/uid block)))}
           (:block/string block)]))
		])))

(defn test2 [{:keys [block-uid]} & args]
  (let [*my-children (dr/pull '[{:block/_refs ...}
                                {:block/children ...} 
                      :block/string 
                      :block/uid] 
                      [:node/title "TODO"])]
    (js/console.log args)
    (fn [& args]
      [:div 
        (doall (for [block (rest (tree-seq :block/uid :block/_refs @*my-children))]
          [:button.bp3-card.green
           	{:style {:background-color (rand-nth color)}
             :on-click (fn [e] (js/alert (:block/uid block)))}
           (:block/string block)]))
		])))``` 
                - ```clojure
(defn page-by-node-title [name] 
  	(dr/pull '[{:block/_refs ...}
               {:block/refs ...}
               {:block/children ...}
               {:block/path ...}
               :block/string 
               :block/uid 
               :block/props
              ]
             [:node/title name])
  )``` [*](((N5iOmzEp3)))
                - ```clojure

(defn my-view [{:keys [:block/uid] :as this-block}]  	
  (let [my-local-string (r/atom "hello")
          my-local-number (r/atom 0)]
      (fn [this-block]
        	[:div.bp3-card 
             "I am a div"

             ""
             (pr-str color)
             (for [x (range 2)]
             [counter my-local-number])
             [controlled-input my-local-string]
             [controlled-input my-local-string]])))


(defn last-render [{:keys [:block/uid] :as this-block}]  	
  (let [my-local-string (r/atom "hello")
          my-local-number (r/atom 0)]
      (fn [this-block]
        	[:div.bp3-card 
             "I am a div"

             ""
             [all-descendents-as-cards 
              @(*page-with-children-by-node-title "roamhacker")]
            ])))
```
                - ```clojure
(defn random-n-refs [n ent]
  	(take n (set (:block/_refs ent))
  ))```
                - ```clojure
(defn *pull-refs [block-uid]
  	(dr/pull '[{:block/_refs ...}
               :node/title
               :block/string
               :block/uid]
             block-uid)
  	
  )```
                - ```clojure

(defn show-refs [component n x]
[:div  
 (doall (for [y (take @n (:block/_refs @x))]
  [component y]))]
  )

(defn my-item [data]
  	[:div.bp3-card (:block/string data)]
  )

(defn my-random-generator [{:keys [:block/uid] :as this-block} n v]  	
  (let [my-local-string (r/atom v)
          my-local-number (r/atom (js/parseInt n))]
      (fn [this-block n v]
        	[:div.bp3-card 
             "I am a div"

             ""
             (pr-str v)
             [counter my-local-number]
             [controlled-input my-local-string]
            
             [show-refs my-item 
              my-local-number 
              (*pull-refs [:node/title @my-local-string])]
             ])))
``````
            - `r/atom` gives you a local variable
            - Final function in your namespace is what gets called with `roam-render`
                - {{roam/render: ((77PX5-Y0t))}}
                    - a
                    - {{[[TODO]]}} Show how to hide all child blocks
                    - {{[[TODO]]}} Inline components?
