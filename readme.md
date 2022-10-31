* Array 
	* [[24_oct_2022#Two Sum]]
		return two value that sum to target value 
		[`a+b = result === result - a = b` store index of element to map with key of `result - a` which is `b`. with that search in array where `b`]
		
	* [[24_oct_2022#Valid Parentheses]]
		checking string if bracket is valid
		[by using stack to check]
		[by using map and stack check if open bracket save close to stack if pop same close then is true]
		
	* [[25_oct_2022#Search Insert Position]]
		return position of a number in un-decresing order of number array
		[using binary search which is using two pointer left and right]
		
	* [[29_oct_2022#Best Time to Buy and Sell Stock]]
		return max profit of time buy and sell
		[is by set up two pointer(buy pointer & sell pointer) where both start at day 0 then sell pointer gradually move if profit check max profit else pointer buy move up]
		
	* [[29_oct_2022#Single Number]]
		search in the array if any number is unique
		[my solution is by put every value in map and count it and return the one with 1 count]
		[Using XOR operator, XOR cancel out same bit so unique bit remain]
		
	* [[30_oct_2022#Majority Element]]
		return majority element in array
		[store each element as key and count each apearing then return the element that apears more than `⌊n / 2⌋` times]
___

* Linked List
	* [[25_oct_2022#Merge Two Sorted Lists]]
		merging two node by arrange in order
		[merging two linked un-decreasing order linked list is done by check every node if bigger then put at the next of smaller]
		
	* [[30_oct_2022#Linked List Cycle]]
		check if a linked is having loop or cycle
		[by change the node value we can know when the same node appear again]
		[we setup two pointer by using tortoise and the hare algorithm]
		
	* [[30_oct_2022#Intersection of Two Linked Lists]]
		given two different linked but it has a same intersection in the end 
		return the intersection
		[by a+b = c === b+a = c; with iterate linked a + b and linked b + a, the end of linked is the intersection]
		[using two pointer for each linked list, we check each and save the node and each pointer check if the node is present then that is the intersection]
	
	* [[30_oct_2022#Reverse Linked List]]
		return linked list in reverse
		[my solution is by cache next of next current node after that change next node next to current node and recursively]
		
	* [[31_oct_2022#Palindrome Linked List]]
		find if a linked list is palindrome
		[find middle linked by using tortoise and the hare algorithm then reverse half of it and then compare of each half]
		
___

* Binary Tree
	* [[26_oct_2022#Binary Tree Inorder Traversal]]
		Given the `root` of a binary tree, return _the inorder traversal of its nodes' values_.
		[This is implementation of In-order Traversal]
		
	* [[27_oct_2022#Symmetric Tree]]
		check if binary tree is symetrical on its root
		[This A Level-Order (Breadth-First) Traversal implementation By Check far left is equal to far right]
		
	* [[29_oct_2022#Maximum Depth of Binary Tree]]
		return the maximal depth of a binary tree
		[My solution is by using Post Order Transversal It takes a “left-right-root” order]
		
	* [[31_oct_2022#Invert Binary Tree]]
		return invert of a binary tree
		[for this problem can be solve by using Level-Order (Breadth-First) Traversal for each node in queue we switch branch]
		
___

* Misc
	* [[26_oct_2022#Climbing Stairs]]
		there a to way to step up 1 step or 2 step. how many combination to if a stairs is `n`
		[using Fibonacci Number Formula ]
* 