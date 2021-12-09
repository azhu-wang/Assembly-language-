# Assembly-language-Bubble Sorting
目的:
宣告一個陣列大小為i的資料(SortData)，其值00~0FH之任意數。再寫一個巨集或副程式，名稱為sort，將SortData 由大排到小，並將結果輸出到螢幕上

原理:
利用泡沫排序法(Bubble Sorting)從陣列的最前面開始，一次比較陣列中兩個最近的相鄰元素，然後根據大小將它們調換順序，小的移到後面：
1.	當我們比較過所有元素一次後，可以確保數值最小的元素在最後面
2.	接著扣掉剛剛陣列中最後面的一個元素（因為已經確定它是最小的），接著重複上面的步驟進行比較
3.	重複上述動作，直到排序完畢。
4.	
Purpose:
Declare a data (SortData) with an array size of i, whose value is any number from 00 to 0FH. Write another macro or subprogram named sort, sort the SortData from large to small, and output the result to the screen

principle:
Use Bubble Sorting to start from the front of the array, compare the two nearest adjacent elements in the array at a time, and then switch them in order according to the size, and move the smaller to the back:
1. After we compare all the elements once, we can ensure that the element with the smallest value is at the end
2. Then subtract the last element in the array just now (because it has been determined to be the smallest), and then repeat the above steps to compare
3. Repeat the above actions until the sorting is completed.

![image](https://user-images.githubusercontent.com/57763355/145403125-3a89ca96-5911-495e-ba40-0f22d5791f72.png)
