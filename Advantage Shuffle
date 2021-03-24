class Solution:
    def advantageCount(self, A, B):
        n = len(A)
        B = sorted([(num, i) for i, num in enumerate(B)])[::-1]
        A = sorted(A)[::-1]
        ans = [-1]*n
        
        beg, end = 0, n - 1
        
        for num, ind in B:
            if A[beg] > num:
                ans[ind] = A[beg]
                beg += 1
            else:
                ans[ind] = A[end]
                end -= 1
                
        return ans
