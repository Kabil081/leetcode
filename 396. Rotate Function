class Solution {
    public int maxRotateFunction(int[] nums) {
        int n = nums.length;
        long F = 0, sum = 0;

        for (int i = 0; i < n; i++) {
            F += (long) nums[i] * i;
            sum += nums[i];
        }

        long maxF = F;

        for (int k = 1; k < n; k++) {
            F = F + sum - (long) n * nums[n - k];
            maxF = Math.max(maxF, F);
        }

        return (int) maxF;
    }
}
