query-table:: false
id:: 681bebcf-ce17-49fc-adf0-1e5ccd57d1d9
query-properties:: [:block :page]
#+BEGIN_QUERY
{:title       "Leisure Tasks"
 :query       [:find (pull ?b [*])
                :where
                ;; match only TODO blocks
                [?b :block/marker "TODO"]
                ;; match blocks that reference the leisure page
                [?b :block/refs ?p]
                [?p :block/name "leisure"]]
 :group-by-page? false
 :collapsed?    false}
#+END_QUERY

-
- #+BEGIN_QUERY
  {:title       "Leisure Tasks (Any Status)"
   :query       [:find (pull ?b [*])
                  :where
                  ;; match blocks that link to [[leisure]]
                  [?b :block/refs ?p]
                  [?p :block/name "leisure"]
                  ;; match any block.marker (i.e. any task status)
                  [?b :block/marker ?m]]
   :group-by-page? false
   :collapsed?    false}
  #+END_QUERY
-
- {{query (and (task TODO) [[leisure]])}}
-
-
- # Reset Relax Tasks
  {{query (and (task DONE) [[relax]])}}
-