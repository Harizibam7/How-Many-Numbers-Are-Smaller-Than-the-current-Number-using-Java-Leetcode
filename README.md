# How-Many-Numbers-Are-Smaller-Than-the-current-Number-using-Java-Leetcode

    class Solution {
        public int[] smallerNumbersThanCurrent(int[] nums) {
            int arr[];
            arr = new int[nums.length];
            for(int i =0; i<nums.length;i++){
                    int count=0;
                    for(int j =0;j<nums.length;j++){
                        if(nums[i]>nums[j] && (j!=i)){
                            count=count+1;
                        }
                    }
                    arr[i]= count;
                    count =0;
    
            }
            return arr;
        }
    }
