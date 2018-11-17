# Comparision Of Two Lists

This repository that contains the code for comparing two lists

### Table of Contents
* [Getting Started](#getting-started)
* [Prerequisites](#prerequisites)
* [Installing](#installing)
* [Python code for Creating Directory](#python-code-for-creating-directory)
* [Approach Towards The Development of Code](#approach-towards-the-development-of-code)
* [Built With](#built-with)
* [Author](#author)

## Getting Started

These instruction will get you a copy of the project up and running on your local machine for development and testing purposes. 

### Prerequisites
* [Python Text editor](https://www.python.org)

If you donot have python text editor ,you can install anaconda In anaconda you have two types of text editors Jupyter Notebook and Spyder

* [Ananconda cloud](https://anaconda.org)

Jupyter Notebook can be installed  without downloading anaconda by using pip

```pip install jupyternotebook```

### Installing
* After downloading install the binaries
* Then add python to system environment variables
* Then install pip
* Using pip install virtualenv(optional)

### Python code
```
import sys,ast
first_list_elements=ast.literal_eval((sys.argv[1]))
second_list_elements=ast.literal_eval((sys.argv[2]))
common_list_elements=list(set(first_list_elements) & set(second_list_elements))
first_list_only=list(set(first_list_elements)-set(second_list_elements))
print(common_list_elements)
print(first_list_only)
```
**Execution**
```
G:\>python prg2.py ['a','b','c'] ['b','d']
['b']
['c', 'a']
```
### Approach Towards The Development of Code

**PROBLEM IN COMPARING OF TWO LISTS**

1. If you use operator between two lists (for extracting common elements or for extracting elements present in L1 and not in L2), it gives you typeerror representing Unsupported operands
2. USing for loop and if clause increase the lines of codes or width of the code

**APPROACH TOWARDS THE PROBLEMS**

1. Converting the list into set and appling required operator between the two sets,later converting set into the list
2. For getting common elements into list convert the list into set and then apply intersection function on it.

### Built With
* [Python Text editor](https://www.python.org)

### Author 

Mounika Mandha

### Thank You
