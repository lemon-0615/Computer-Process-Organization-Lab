# Lab for  Computer Process Organization

### Lab1

#### Title:
  Computational Process Organization Lab1,variant 1

#### List of group members:
  - Name:Huang Yanlin,  student number:192050222 [lemon-0615](https://github.com/lemon-0615)
  - Name:Lin ningning,  student number:192050192  [Lin-12](https://github.com/Lin-12)

#### Laboratory work number:
   Lab1 variant 1
#### Description:
   variant 1: Unrolled linked list (you can use built-in list inside node).

#### Synopsis:  
* add a new element (lst.add(3), cons(lst, 3), extend(lst, 3));  
* remove an element (lst.remove(3), remove(lst, 3));
* size (lst.size(), size(lst));    
* conversion from and to python lists (lst.to_list(), lst.from_list([12, 99, 37]), from_list([12, 99, 37]));   
* find element by specific predicate (lst.find(is_even_), );    
* filter data structure by specific predicate (lst.filter(is_even));   
* map structure by speci?c function (lst.map(increment));   
* reduce-process structure elements to build a return value by speci?c functions (lst.reduce(sum));    
* data structure should be a monoid and implement mempty and mconcat functions or methods;    
* iterator: 
   - for the mutable version in Python style [12, Chapter 7. Classes & Iterators]; 
   - for the immutable version by closure [14], see example ahead.

#### contribution
* contribution summary for each group member (should be checkable by git log and git blame);
   - mutable&test_mutable:Lin ningning 
   - immutable&immutable_test:Huang Yanlin 
#### Explanation：  
  Unrolled linked list is a kind of transformation or improvement of linked list. Each node of it is stored by an array. The capacity of node array is fixed. 1. Insert operation: insert the element after finding the position according to the subscript. If the current inserted node array is full, a new node is created, and half of the elements of the current node are moved to the array of the new node, and the element is inserted finally. 2. Delete: delete the element according to the subscript. A node after deleting an element may need its neighbors to merge. Unrolled linked list has the advantages of random access of array and efficient insertion and deletion of linked list.

#### Work demonstration 
* (how to use developed software, how to test it), should be repeatable by an instructor by given command-line examples:  
  - We write unrolled linked list file and test file on Pycharm.
  - Use terminal to test the code. like 'python Immutable_test.py -v'and 'python test_mutable.py -v'.

#### Conclusion:  
  Mutable version used used list to create a unrolled linked list.In immutable version,we create a new unrolled linked list before modifying each unrolled linked list, and do not change the original linked list.This Lab makes us to realize unrolled linked list and  mutable/immutable version.

### Lab2

#### Title:
  Computational Process Organization Lab2,variant 6

#### List of group members:
  - Name:Huang Yanlin,  student number:192050222 [lemon-0615](https://github.com/lemon-0615)
  - Name:Lin ningning,  student number:192050192  [Lin-12](https://github.com/Lin-12)

#### Laboratory work number:
   Lab2 variant 6
#### Description:
   variant 6: Regular expression

#### Synopsis:  
* Support special characters: \, ^, ., $, *, +, [ ], [^ ], { }.  
* Support functions: match, sub.
* Visualization as a finite state machine (state diagram or table).    

#### contribution
* contribution summary for each group member (should be checkable by git log and git blame);
   - lexer.py & regex.py:Huang Yanlin
   - nfa.py : Lin ningning
   - sample.py :HuangYanlin & Lin ningning

#### Explanation：  
 * lexer
    - Lexical analysis of regular expressions
 * regular
    - About some functions for Regular expression
 * nfa
    - Definition of an NFA node the construction of an NFA
 * sample
    - About some test for Regular expression

#### Work demonstration 
* (how to use developed software, how to test it), should be repeatable by an instructor by given command-line examples:  
  - We write all files on Pycharm.
  - Use terminal to test the code. like 'python sample.py -v'.

#### Conclusion:  
  * We implement simple library for RE and demonstrate how it works.
  * This lab is difficult for us but we also learn more about it.
  * We add some practical examples in tests which make this code to have practical meanings.

### Lab3

#### Title:
  Computational Process Organization Lab3,variant 1

#### List of group members:
 - Name:Huang Yanlin,  student number:192050222 [lemon-0615](https://github.com/lemon-0615)
 - Name:Lin ningning,  student number:192050192  [Lin-12](https://github.com/Lin-12)

#### Laboratory work number:
   Lab3 variant 1
#### Description:
   variant 1: In this variant, you should implement a lazy library for a single-linked list. For that, you should use closures. Usage of generators (yield statement) or async (async, await statements) is not allowed.

#### Synopsis:  
 implement the following API:
 
* head(List) – return a list first element. If the list is empty – raise an exception. 
* tail(List) – return tail of the list.
* length(List).
* map(List, Function) and reduce(List, Function, InitialState).
* mempty().
* mconcat(List1, List2) – should not force list evaluation.
* from_list(pythonList) and to_list(List).
* it should be an iterator.
* Complex test – factorial
   - To proof correctness, use unit tests, properties-based tests
   - To proof laziness,demonstrate it for all suitable implemented functions on an infinite list (e.g. natural numbers sequence) and a 

#### contribution
* contribution summary for each group member (should be checkable by git log and git blame);
   - Linkedlist:Huang Yanlin
   - Linkedlist_test:Lin ningning

#### Explanation：  
  we create a single-linked list and use closures.And we not use  generators (yield statement) or async (async, await statements).
  
#### Work demonstration 
* (how to use developed software, how to test it), should be repeatable by an instructor by given command-line examples:  
  - We write Linkedlist file and test file on Pycharm.
  - Use terminal to test the code. like 'python Linkedlist.py -v'and 'python Linkedlist_test.py -v'.

#### Conclusion:  
  We create a single-linked list and use closures.It's easy to see the test result.
  
 


