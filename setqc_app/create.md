# Create a setQC report 

## To create a setQC report in the app, you need the following : 

* The libraries need to be stored in the metaData app 
* `PE` and `SE` for each lib need to be correctly indicated to allow
  the app correctly to search for `r1/2` or not `r2` reads. 
  


## To created a report including `pooled` libraries: 

* Use the `_1_2` convention to indicated which sequecing run from this
  library to pool. For example, `JYH_123_1_2` means you are going to
  pool sequencing runs `JYH_123` and `JYH_123_2` togather.
  
* Notice that the first sequecing from a library we **don't** use `_1`
  to indicate that because not all libraries will sequece more than 1
  time. So no `JYH_123_1` for the first sequencing for library
  `JYH_123`. 
  
* Again, for any the pooled sequecing (e.g. `JYH_123_1_2`), it is also required
  to create pseduo-sequecing sequecing with the pooled id
  (e.g. `JYH_123_1_2`) in the metaData app to allow setQC app to call.
  
  
  
