Longest Consecutive Subsequence
Here on this page, we will learn to create Python Program to find Longest Consecutive Subsequence.

Example :

Input : [7, 8, 1, 5, 4, 3]
Output : 3
Python Program for Longest Consecutive Subsequence

Algorithm
Initialize Empty array val and a variable c with value zero
Iterate using a for loop between range zero to l with variable i
Initialize a variable n with value 1
Use a nested while loop until arr[i]+n in arr
for each iteration increment the value of c & n by 1
Append c+1 in val
set value of c to 0
print maximum of val
Longest Consecutive Subsequence in Python
Python Code
Run
def LongestConseqSubseq(arr, l):
    val = []
    c = 0
    for i in range(l):
        n = 1
        while arr[i] + n in arr:
            c += 1
            n += 1
        val.append(c + 1)
        c = 0
    return max(val)


array = [7, 8, 1, 5, 4, 3]

print("Longest Consecutive Subsequence :", LongestConseqSubseq(array, len(array)))
Output
Longest Consecutive Subsequence : 3
