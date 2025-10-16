class Solution {
    public int findSmallestInteger(int[] nums, int value) {
        int n = nums.length;
        int[] count = new int[value];
        for (int num : nums) {
            int mod = ((num % value) + value) % value;
            count[mod]++;
        }
        int mex = 0;
        while (true) {
            int mod = mex % value;
            if (count[mod] == 0) break;
            count[mod]--;
            mex++;
        }
        return mex;
    }
}
