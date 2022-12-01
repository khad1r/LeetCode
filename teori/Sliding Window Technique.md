**Window Sliding Technique** is a computational technique which aims to reduce the use of nested loop and replace it with a single loop, thereby reducing the time complexity.

**Prerequisite to use Sliding window technique**

The use of Sliding Window technique can be done in a very specific scenario, where the **size of window** for computation is **fixed** throughout the complete nested loop. Only then the time complexity can be reduced. 

**How to use Sliding Window Technique?**

The general use of Sliding window technique can be demonstrated as following:

1.  Find the size of window required 
2.  Compute the result for 1st window, i.e. from start of data structure
3.  Then use a loop to slide the window by 1, and keep computing the result window by window.

**Examples to illustrate the use of Sliding window technique**

**Example:** Given an array of integers of size **‘n’,** Our aim is to calculate the maximum sum of **‘k’** consecutive elements in the array.

> Input  : arr[] = {100, 200, 300, 400}, k = 2  
> Output : 700
> 
> Input  : arr[] = {1, 4, 2, 10, 23, 3, 1, 0, 20}, k = 4   
> Output : 39  
> We get maximum sum by adding subarray {4, 2, 10, 23} of size 4.
> 
> Input  : arr[] = {2, 3}, k = 3  
> Output : Invalid  
> There is no subarray of size 3 as size of whole array is 2.

**Naive Approach:** So, let’s analyze the problem with **Brute Force Approach**. We start with first index and sum till **k-th** element. We do it for all possible consecutive blocks or groups of k elements. This method requires nested for loop, the outer for loop starts with the starting element of the block of k elements and the inner or the nested loop will add up till the k-th element.

Consider the below implementation : 

-   C++
-   C
-   Java
-   Python3
-   C#
-   PHP
-   Javascript

**Sliding Window Technique:** The technique can be best understood with the window pane in bus, consider a window of length **n** and the pane which is fixed in it of length **k**. Consider, initially the pane is at extreme left i.e., at 0 units from the left. Now, co-relate the window with array arr[] of size n and pane with current_sum of size k elements. Now, if we apply force on the window such that it moves a unit distance ahead. The pane will cover next **k** consecutive elements. 

**Applying sliding window technique** : 

1.  We compute the sum of first k elements out of n terms using a linear loop and store the sum in variable window_sum.
2.  Then we will graze linearly over the array till it reaches the end and simultaneously keep track of maximum sum.
3.  To get the current sum of block of k elements just subtract the first element from the previous block and add the last element of the current block .

The below representation will make it clear how the window slides over the array.  
 

> Consider an array **arr[]** = {5, 2, -1, 0, 3} and value of **k** = 3 and **n** = 5
> 
> This is the initial phase where we have calculated the initial window sum starting from index 0 . At this stage the window sum is 6. Now, we set the maximum_sum as current_window i.e 6.   
>  
> 
> ![](https://media.geeksforgeeks.org/wp-content/uploads/sliding-window1.png)
> 
> Now, we slide our window by a unit index. Therefore, now it discards 5 from the window and adds 0 to the window. Hence, we will get our new window sum by subtracting 5 and then adding 0 to it. So, our window sum now becomes 1. Now, we will compare this window sum with the maximum_sum. As it is smaller we wont the change the maximum_sum.   
>  
> 
> ![](https://media.geeksforgeeks.org/wp-content/uploads/sliding-window2.png)
> 
> Similarly, now once again we slide our window by a unit index and obtain the new window sum to be 2. Again we check if this current window sum is greater than the maximum_sum till now. Once, again it is smaller so we don’t change the maximum_sum.  
> Therefore, for the above array our maximum_sum is 6.
> 
> ![](https://media.geeksforgeeks.org/wp-content/uploads/sliding-window3.png)