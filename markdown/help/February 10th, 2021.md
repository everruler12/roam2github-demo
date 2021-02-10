- Example of using query in the roam/render component
    - {{roam/render: ((Mfk6Jol2T))}}
    - ```clojure
(ns myns
  (:require 
   [reagent.core :as r]
   [datascript.core :as d]
   [roam.datascript.reactive :as dr]))

(defn query-list [x]
  (let [y (dr/q '[:find ?e 
                  :in $ ?title
                    :where [?e :node/title ?title]]
                x
                )]
    
  (fn [x]
    [:div (pr-str @y)]
    )  
  )
  )

(defn input-thing []
  	(let [x (r/atom "TODO")]
 		(fn []
            [:div 	
              [:input {:value @x
              :on-change (fn [e] (reset! x (.. e -target -value)))}]
    	^{:key (str @x)}[query-list @x]]
          )))```
