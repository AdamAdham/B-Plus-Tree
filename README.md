# B+ Tree

B+ trees offer significant value by providing efficient data retrieval in block-oriented storage applications like file systems and databases. A B+ tree is nothing more than a tree (with a particularly high fanout or order, which we shall refer to as _m_) that satisfies the following conditions:

* An internal node (nodes that aren't the root or leaves) must have a number of children _d_ such that &#8968;_m_/2&#8969;	&#8804; _d_ &#8804; _m_
* The root node may have at least 2 children and up to _m_ children
* The number of keys _k_ that an internal node may carry is &#8968;_m_/2&#8969; - 1	&#8804; _k_ &#8804; _m_ - 1 
* Leaf nodes have no children, but the number of dictionary pairs _k_ that a single leaf node may carry is &#8968;_m_/2&#8969; - 1	&#8804; _k_ &#8804; _m_ - 1

A B+ tree is similar to a B tree except that all the dictionary pairs lie in the leaf nodes.

# Adjustments
1. Key of the key value pair is a comparable
2. Value of the key-value pair is an vector of strings (my use case was the names of the pages that was serialized)
<br>

## Authors
* **[Shandy Sulen](https://github.com/shandysulen)**
