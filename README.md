# MergeSort
# Question
16,21,11,8,12,22 -> Merge Sort

Write the steps of the above array according to the sort type.

Write the Big-O notation.

# Answer
Step 1: Split the list in half - [16,21,11,8,12,22] becomes [16,21,11] and [8,12,22]

In the first step, the initial list is split in half to create two sublists: [16,21,11] and [8,12,22]. This is done by dividing the list into two equal parts, or as close to equal as possible.

Step 2: Split the first half of the list in half again - [16,21,11] becomes [16,21] and [11]

In this step, we apply merge sort recursively by splitting the first half of the list in half again to create two more sublists: [16,21] and [11].

Step 3: Split the second half of the list in half again - [8,12,22] becomes [8,12] and [22]

In this step, we repeat the process from step 2 by splitting the second half of the list in half again to create two more sublists: [8,12] and [22].

Step 4: Compare and merge the two sublists from step 2 - [16,21] and [11] become [11,16,21]

In this step, we compare each element from the left and right half of the sublists and sort them in the correct order. So [16,21] and [11] become [11,16,21].

Step 5: Compare and merge the two sublists from step 3 - [8,12] and [22] become [8,12,22]

In this step, we repeat the process from step 4 by comparing each element from the left and right half of the sublists and sort them in the correct order. So [8,12] and [22] become [8,12,22].

Step 6: Compare and merge the two sublists from step 4 - [11,16,21] and [8,12,22] become [8,11,12,16,21,22]

In this step, we compare and merge the two sorted sublists from step 4 and 5. This is done by comparing the first element of each sublist and adding the smaller element to the final list, then repeating the process until all elements have been added. So [11,16,21] and [8,12,22] are merged to become [8,11,12,16,21,22].

At this point, the final list is fully sorted and the process is complete. The final list is [8,11,12,16,21,22].

Big-O notation

The time complexity of merge sort is O(n * log n) where n is the number of elements in the input list. This is because the algorithm splits the input list into two sublists at each level of recursion and then merges the sublists back together. The number of splits is logarithmic in nature, so it takes log n steps to split the list into individual elements. And on each step, it takes n steps to merge the two sublists back together, resulting in a time complexity of O(n * log n). It's also worth noting that the space complexity of merge sort is O(n) because it uses temporary arrays to store the sublists during the merging process.





