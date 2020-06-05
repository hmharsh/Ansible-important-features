# Custom python module implementation in ansible 
## Module path(in ubuntu vm): /usr/lib/python2.7/dist-packages/ansible/modules/

## we can add custome module also to:
-  any directory added to the ANSIBLE_LIBRARY environment variable ($ANSIBLE_LIBRARY takes a colon-separated list like $PATH)
-  ~/.ansible/plugins/modules/
-  /usr/share/ansible/plugins/modules/
or simple just put it into in directory named directory under current directory where aisble playbook is present

```To import library (like 'os' etc) in python code from custom module, import from file:  cat /usr/lib/python2.7/dist-packages/ansible/module_utils/bac.py // where different functions are there for different usecases,```
for more details
refer: https://medium.com/@heenashree2010/create-a-custom-module-with-ansible-python-6285874a09b4#:~:text=Write%20your%20first%20python%20program&text=The%20testing.py%20module%20utility,%2C%20import%20from%20testing.py.&text=This%20will%20import%20all%20the,python%20file%20is%20only%20JSON.


##  1.yml: basic implementation 
## 2.yml: implementation where python code having import statements
