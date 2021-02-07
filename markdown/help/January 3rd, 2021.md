- [[Conor]]
    - {{[[DONE]]}} 18:07 - 18:14
        - Basic Key Commands
            - `Command .` zoom in
            - `Command ,` zoom out
        - Other Basics
            - Block references 
            - showing references
            - Multi Select 
    - 18:15 - 18:34
        - # {{[[DONE]]}} [[Goal]] Create a button that alerts hello world
            - {{iframe: https://www.loom.com/embed/4f546ce050d04db993aa63832975e7dc}}
            - {{[[DONE]]}} Call a block with [[roam/render]] 
                - Steps::
                    - `{{[[roam/render]]: ((type something in here and hit create as blok below))}}`
                        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froamex%2FoXTa_JK0aX.png?alt=media&token=c83cc163-7aa4-4afc-af95-d449c75175ee)
                - Result:: Should look like this ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froamex%2FBTRVlUfOCV.png?alt=media&token=69ba2286-e8b4-4875-8fe9-57ccec74cee4)
            - {{[[DONE]]}} Turn on custom components
                - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froamex%2F8VIIDI9MWA.png?alt=media&token=ca537c3b-4550-4968-a449-9ca037101fe9)
                - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froamex%2FJsjcGzNVPm.png?alt=media&token=d1bb3008-378e-42b9-b861-33501ccee40d)
            - {{[[DONE]]}} Write a clojure block
            - 18:16 - 18:36 (20 min)
                - {{[[roam/render]]: ((w0tJtUOLy))}}
                    - {{[[roam/render]]: ((J4WWqA_he))}}
                    - Block to call ```clojure
(defn my-component [_]
  	[:div {:on-click (fn [e] (js/alert "Hello Mason"))
           :style {:background-color "red"
                   :font-size "40px"
                   :color "rgb(245,245,255)"}}
     
     "Hello Friend"]
  )```
        - 
    - # [[Goal]] Create a counter button
        - {{iframe: https://www.loom.com/embed/c937d4c551ad4ebe9db049d174f8b350}}
        - 18:38 - 19:19 (40 minutes)
            - Concepts to explain
                - {{[[DONE]]}} How namespaces in Roam currently work
            - {{[[DONE]]}} Include the reagent namespace libraries
                - {{[[DONE]]}} `(ns )`
                - {{[[DONE]]}} `(:require)`
            - {{[[DONE]]}} Learn some clojure functions for changing an atom
                - {{[[DONE]]}} `swap!`
                - {{[[DONE]]}} `reset!`
                - {{[[DONE]]}} `@`
        - 18:39 - 18:52 (12 min)
            - [[User Error]] - from [[Conor]] -- which points to [[Confusion]]
                - The block you call has to have a function in it --  but it will load the namespace from all of it's sibling blocks
                - Scratch work
                    - Attempt 1
                        - {{[[roam/render]]: ((g4w4v6tkq))}}
                        - Counter Button file ```clojure
(ns mynamespace1
  (:require [reagent.core :as r]))

(defn x [_]
  [:div "hey"])```
                        - ```clojure
(defn counter [_]
  	[:button "hello from here"]
  )```
        - 18:55 - 19:18
            - "{{[[DONE]]}} How namespaces in Roam currently work"
                - # Counter File
                    - ```clojure
(ns my-namespace 
  (:require [reagent.core :as r]))```
                    - ```clojure
(defn inc-button [count-atom]
[:button.bp3-button  {:on-click (fn [e] 
                 (swap! count-atom inc))
          		}	"Inc"]
  )```
                    - Different Block to call ```clojure

(defn my-differant component [_]
    (let [magic-number (r/atom 42000)]
      (fn [_]
    	   [:div { :style {:background-color "#F44336"
            
                   :color "#fff"}} @magic-number
     		[:div 
             
             [:button.bp3-button.bp3-minimal 
              {:on-click (fn [e] 
                 (swap! magic-number (partial + 10)))
          		}	
     
    	 "Add 10" ]]])))```
                    - Block to call ```clojure
(defn my-component [_]
(let [magic-number (r/atom 42)]
  (fn [_]  
    [:div {
           :style {:background-color "green"
                
                   :color "#fff"}}
     
     [:button.bp3-button  {:on-click (fn [e] (reset! magic-number "Hey Adam"))}
     "Reset to Zero"]
     [inc-button magic-number]
     @magic-number])))```
                - Calling it
                    - {{[[roam/render]]: ((KAVRdGHut))}}
                    - {{[[roam/render]]: ((SGUEGZaZn))}}
