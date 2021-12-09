# Assembly-language-Bubble Sorting

Purpose:
Declare a data (SortData) with an array size of i, whose value is any number from 00 to 0FH. Write another macro or subprogram named sort, sort the SortData from large to small, and output the result to the screen

principle:
Use Bubble Sorting to start from the front of the array, compare the two nearest adjacent elements in the array at a time, and then switch them in order according to the size, and move the smaller to the back:
1. After we compare all the elements once, we can ensure that the element with the smallest value is at the end
2. Then subtract the last element in the array just now (because it has been determined to be the smallest), and then repeat the above steps to compare
3. Repeat the above actions until the sorting is completed.
