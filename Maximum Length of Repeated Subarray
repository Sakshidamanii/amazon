class Solution {
	public int findLength(int[] nums1, int[] nums2) {
		int[] curr = new int[nums2.length + 1];
		int[] prev = new int[nums2.length + 1];
		int max = 0;
    
    for(int i=1;i<=nums1.length;i++){
        for(int j=1;j<=nums2.length;j++){
            if(nums1[i-1] == nums2[j-1]){
                curr[j] = prev[j-1] + 1;
                max = Math.max(curr[j], max);
            }
        }
        prev = curr.clone();
        curr = new int[nums2.length + 1];
    }
    
    return max;
	}
}
