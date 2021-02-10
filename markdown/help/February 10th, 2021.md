- 
- {{roam/render: ((Mfk6Jol2T))}}
- ```clojure
(ns myns
  (:require 
   [reagent.core :as r]
   [datascript.core :as d]
   [roam.datascript.reactive :as dr]))

(defn x []
  	(r/with-let [x (r/atom "TODO")]
	[:div 
     [:input {:value @x
              :on-change (fn [x] (reset! x (.. x -target -value)))}]
     (pr-str @(dr/q '[:find ?e 
                           :where [?e :node/title "TODO"]]))]))```
