# iOS-Tensorflow-for-Poets

Xcode iOS App that uses Google Tensorflow API to identify flowers

Directions:  first unzip the "pods.zip" file then run "tflite_photos_example.xcworkspace"

Sources:

https://codelabs.developers.google.com/codelabs/tensorflow-for-poets/index.html?index=..%2F..index#0

https://codelabs.developers.google.com/codelabs/tensorflow-for-poets-2-ios/index.html?index=..%2F..index#0

Notes:

* Change this line

  #include "tensorflow/contrib/lite/tools/mutable_op_resolver.h"

  to this line

  #include "tensorflow/contrib/lite/op_resolver.h"

* TOCO Issue

  Replace:
  
    --graph_def_file=tf_files/retrained_graph.pb
    
    with:
    
    --input_file=tf_files/retrained_graph.pb
