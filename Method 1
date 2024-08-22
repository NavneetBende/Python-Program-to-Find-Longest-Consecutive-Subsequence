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
