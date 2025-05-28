- ```query  
  {:title "Errands"  
   :query [:find (pull ?b [:block/content :block/marker :block/page :block/properties])  
           :where  
           [?b :block/refs [:block/name "errand"]]  
           (or  
             [?b :block/marker "TODO"]  
             [?b :block/marker "DOING"])]}  
  ```
-
- {{query (and [[Errand]] (task TODO DOING))}}
-
-
-