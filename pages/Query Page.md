query-table:: false
#+BEGIN_QUERY
{:title [:b "最近7天有更新的页面"]
 :query [:find (pull ?p [*])
         :in $ ?start ?today
         :where
         [?p :block/updated-at ?d]
         [(>= ?d ?start)]
         [(<= ?d ?today)]
         [?b :block/page ?p]
         ]
 :inputs [:7d-before-ms :end-of-today-ms]
}
#+END_QUERY

-