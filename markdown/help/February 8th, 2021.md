- [[Hiring]] [[Work at Roam]] [[Clojure Engineer]] - [[Backend Role]] [[Take Home Project]]
    - Given two Roam Trees
        - 
        - {{roam/render: ((uP_2barEP))}}
            - ```clojure
(ns starting-point-for-custom-roam
  (:require
   [reagent.core :as r]
   [datascript.core :as d]
   [roam.datascript.reactive :as dr]))

(defn x [{b :block-uid}]
  	[:div (pr-str @(dr/pull '[*] [:block/uid b]))]
  )```
