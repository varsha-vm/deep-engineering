# Indexing in SQL
- Indexing is a data structure creayed by SQL developers to make the query execution faster.
- Indexing create a copy on data and uses seperate disk space to hold  indexed data, hence it can be redundant.
- Real life example would be the index available on back of every book with page numbers.
- Indexing make query execution easier as everything is ordered just like content in yellow pages or telephone directory.
- Indexing under the hood is build using two data structures such as doubly linked list & BST tree.
- Indexing is expensive and hard, due to underlying data changes such as insert, update & delete will have to make changes to existing data position in place.
- Indexing is a smarted way of accessing data. Basically it is a data structure that stores column value in searchable order,  along with its pointer to actual rows.
- Indexing is very useful for read than write. 
    - Reads are efficient w/ indexing as it directly locates to the index that the data range recides in and fetches the data.
    - Write can get slow and expensive as the data will have to be moved, update, splitted, pointers need to be changed etc.
- With Indexing, full data scan can be avoided (Select *) as the data is ordered with indexing and fecting column data gets faster.
- Advantages:
    - Tables store actual data, where as indexes store order of the data.
    - Reads are faster
- Disadvantages:
    - Pay for Writes
    - Disk I/O increases with Writes as the data need to be written, then the order need to be changed, stored, updated for indexing.
- Indexing best practices:
    - Indexing few good columns is always better than more columns.
    - Indexed columns are mostly used in WHERE, JOIN, ORDER BY.
    - Columns that changes values frequently like timestamp etc are not good candidate for indexing.
    - Do not index small tables as DB will full scan anyways and no use of indexing here.
    




