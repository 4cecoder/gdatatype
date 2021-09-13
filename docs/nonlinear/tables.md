# Tables

### Simple Table
A simple way to implement a table is by using an array. Each element in the array can store one record. The records in the array are kept sorted according to the key. Note that a table does not have to have an ordering. The sorting of the keys just helps to make certain functionality faster

### Insertion/Update
To add to this table, we must first find the spot where the item will go. This can be done by modifying a binary search algorithm. Once the location is found, if a record with the same key is not already in the table, we will need to shift every item over to make room for the new record. If a record with a matching key already exists, the old record can be replaced with the new.

The run time for performing the search is O(log n). If the record already exists, and we are just updating it, the run time would be O(log n). However, inserting a brand new record with a different key will require shifting on average 50% of the list, and thus we are looking at a run time of O(n) for that operation.

### Remove
To remove a record, we can start with a binary search algorithm to find the record according to the key. If such a record exists, removal will involve shifting the records down.

The run time for search is O(log n). However to remove, we must shift all the records down. This process is O(n). Thus the remove operation is O(n)

### Search
As the array is sorted by key, all searching can be done using a binary search. This has a run time of O(log n)
