# Pure python MVC design pattern example #

Example of the `MVC` (Model View Controller) design pattern on pure Python. 
Writen for "Use Python in the Web" course of `IMKN` (Institute Mathematics and 
Computer Science) at `UrFU` (Ural Federal University) in `2015` by `Pavel Blinov`

Old version: https://github.com/pahaz/Example-of-MVC-pattern-on-pure-Python-2014

 - WSGI and WebServer: `wsgi.py`, `server.py`
 - Model: `model.py`, `manager.py`
 - View: `view.py`
 - Controller: `controller.py`, `router.py`

# coupling #
                                                                     
                                                  +---------------+  
     +-------------+          +------+            |   +-------+   |  
     | application |          | view | -------------> | model |   |  
     +-------------+          +------+            |   +-------+   |  
            |                     ^               |       ^       |  
            |                     |               |       |       |  
     +------v---------------------|---------+     |       |       |  
     |  +--------+         +------------+   |     |  +---------+  |  
     |  | router | ------> | controller | ---------> | manager |  |  
     |  +--------+         +------------+   |     |  +---------+  |  
     +--------------------------------------+     +---------------+  
                                                                     
`A -> B`  -- the component A knows the interface of the component B

