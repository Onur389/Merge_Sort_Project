# Merge_Sort_Project
Merge sort project for patika.dev

 Merge sort is an algorithm that is getting used by data scientists. In this algorithm, data set is continuously divided by 2^x data sets and
 sorts between these data sets. It provides us a smaller time complexity and smaller big-o notation but it consumes more storage than insertion sort algorithm.


We have [16,21,11,8,12,22] data set and we need to sort these numbers with merge sort algorithm.


At the first step the data set should be divided by 2:
[16,21,11]  [8,12,22]


At the second step data sets will be divided by 2 too.:
[16,21] [11] [8,12] [22]


Then, we should sort these numbers among 2 data sets:
[16,21] [11] | [8,12] [22]


11 is the smallest and 22 is the biggest. As a result of this, our set have became this:
[11,16,21] | [8,12,22]


Let's check which has the smallest numbers between these two sets.
8 is smaller than 11. 11 is smaller than 12.
[8,11,16,21] [12,22]


16 is bigger than 12 and smaller than 22.
Then we have [8,11,12,16,21] [22]


Finally let's look at 21.
21 is smaller than 22 and we have [8,11,12,16,21,22] data set at the end.



Everytime we look a pattern, total sets degreased n = 2^x times
we have x = nlog2(n) Big-O notation O(nlogn) is better than Insertion sort.





