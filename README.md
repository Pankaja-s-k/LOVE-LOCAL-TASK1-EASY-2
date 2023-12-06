# LOVE-LOCAL-TASK1-EASY-2
1. TreeNode Class:
This class defines the structure of a node in a binary tree.

TreeNode has three properties: val, left, and right.
val stores the value of the node.
left points to the left child node.
right points to the right child node.
2. sortedArrayToBST Function:
This function takes a sorted array nums and constructs a balanced binary search tree from it.

Base Case:

If nums is empty, it returns None as there's no tree to construct.
Finding the Root:

It calculates the index of the middle element of nums (mid = len(nums) // 2).
Creates a TreeNode with the value of the middle element as its val.
Recursion for Left and Right Subtrees:

Recursively calls sortedArrayToBST on the left half of the array (nums[:mid]).
The result becomes the left child of the current root node.
Recursively calls sortedArrayToBST on the right half of the array (nums[mid+1:]).
The result becomes the right child of the current root node.
Returns:

It returns the current root node, which represents the constructed balanced binary search tree.
3. inorderTraversal Function:
This function performs an inorder traversal of the tree, printing the values of nodes in sorted order.

Base Case:

If the root node is None, it stops the traversal.
Inorder Traversal:

Recursively calls itself on the left subtree.
Prints the value of the current node.
Recursively calls itself on the right subtree.
4. Example Usage:
The code provides examples to demonstrate the functionality:

Example 1 (nums1 = [-10, -3, 0, 5, 9]):

Constructs a balanced binary search tree from the provided sorted array.
Prints the inorder traversal of the resulting tree, showing the nodes in ascending order (-10, -3, 0, 5, 9).
Example 2 (nums2 = [1, 3]):

Constructs another balanced binary search tree from the given sorted array.
Prints the inorder traversal of the resulting tree, displaying the nodes in ascending order (1, 3).
