@gf712 Can you please review the following steps to be added in EXAMPLES.md. Thanks in advance :D.
It is extremely simple to add a new example. Just create another `*.sg` file. The following are the steps to port the examples:

1. Add file in ```examples/meta/src/*/*.sg``` (```.sg``` file contains example code in meta-language specific to shogun)  

2. The next step is to build these examples. During build these are parsed and then translated with the (Python) machinery in ```examples/meta/generator/*.py.``` The output is a code listing for each target language defined in ```examples/meta/src/generator/targets/*.json.```   
For python, the command is:   
``` make meta_examples```    
**Note** This is only available when the cmake option BUILD_META_EXAMPLES=ON is set, and the Python requirements in examples/meta/requirements.txt are met.  
For C++, the command is:  
```make build_cpp_meta_examples``` and then run them as from their folder straight-away (you might have to set environmental variables, see INTERFACES.md)  
```
cd examples/meta/cpp/multiclass
./cpp-multiclass-k_nearest_neighbours
```
