# 🚀 Array Transformation (Java)

Optimized Java solution to minimize operations required to make all array elements equal using remainder grouping and median-based optimization.

## 📌 Problem Statement
Given an array of integers A and an integer K, you can perform the following operation any number of times:
- Add or subtract K from any element

Return the minimum number of operations required to make all elements equal.  
If it is not possible, return -1.

## 💡 Approach
1. Remainder Check  
   All elements must have the same remainder when divided by K.  
   If not → return -1  

2. Transform the Array  
   Convert each element:
   B[i] = A[i] / K  

3. Sort the Array  

4. Choose Median  
   Median minimizes total operations  

5. Count Operations  
   operations = Σ |B[i] - median|

## ⚙️ Time & Space Complexity
Time Complexity: O(n log n)  
Space Complexity: O(n)

## 🧪 Example
Input:
5  
55 15 75 45 65  
5  

Output:
16

## 🔍 Explanation
Original Array: [55, 15, 75, 45, 65]  
After division by K: [11, 3, 15, 9, 13]  
Sorted: [3, 9, 11, 13, 15]  
Median = 11  

Operations:  
|3-11| + |9-11| + |11-11| + |13-11| + |15-11| = 16  

## 🧠 Key Insight
Only elements with the same remainder can be transformed.  
Using the median minimizes total operations.

## 📂 Project Structure
ArrayTransformation.java  
README.md  

## 🛠️ Technologies Used
Java  
Arrays & Sorting  
Mathematical Optimization  

## ✨ Author
Bishakha  

## ⭐ Support
If you found this helpful, give it a ⭐ on GitHub!
