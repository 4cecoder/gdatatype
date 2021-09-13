# Containers

 ### is a class or a data structure whose instances are collections of other objects.
     
      - stores objects in an organized way that follows specific access rules.
       
        The size of the container
        - depends on the number of objects (elements) it contains. 
        
        Underlying (inherited) implementations of various container types
        - may vary in size and complexity
        - provide flexibility in choosing the right implementation for any given scenario.



### Containers can be characterized by the following three properties:
    - access, that is the way of accessing the objects of the container. In the case of arrays access is done with the array index. In the case of stacks, access is done according to the LIFO (last in, first out) order and in the case of queues it is done according to the FIFO (first in, first out) order;
    - storage, that is the way of storing the objects of the container;
    - traversal, that is the way of traversing the objects of the container.

### Container classes are expected to implement methods to do the following:

    - create an empty container (constructor);
    - insert objects into the container;
    - delete objects from the container;
    - delete all the objects in the container (clear);
    - access the objects in the container;
    - access the number of objects in the container (count).

Containers are sometimes implemented in conjunction with iterators.   