pythonMixProgramming
====================

It is actually very simple to call a c++ function from python, however, it is always not clear until it become clear.

a very good example can be found at https://scipy-lectures.github.io/advanced/interfacing_with_c/interfacing_with_c.html, while it is not a step by step tutorial.

Let me do it.

1. open visual studio and build a new win32 console project, and the type is not an application, but a dll.
2. select empty project
3. add a source.cpp
4. copy the contents in
5. add include folder C:\python27\include or something similar
6. add additional library folder C:\python27\libs
7. build the project
8. change the output file from dll to pyd from C++ general in options of the project 
9. notice the name of the project should be consistent with Py_InitModule
10. build the project

1. open a cmd
2. python
3. import cos_module
4. cos_module.cos_func(5)


That's all. Simple? Yes, if you have a good tutorial.
