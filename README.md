class Solution {

    public int[] twoSum(int[] nums, int target) {
        int arr[];
        arr= new int[2];
        for(int i=0;i<nums.length;i++){
           int sum=0;
            for(int j=i+1;j<nums.length;j++){

                if(nums[i]+nums[j]==target){
                    arr[0]=i;
                    arr[1]=j;
                }

            }

        }
        return arr;
    }
}


palindrome
class Solution {
    public boolean isPalindrome(int x) {
        int a,b,c;
        b=0;
        a=0;
        c=x;
        while(x>=1){
            a=x%10;
            x=x/10;
            b=10*b+a;
        }
        if(c==b){
            return true;
        }

        else{
            return false;

        }



    }
}
