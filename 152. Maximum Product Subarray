class Solution {
public:
    int maxProduct(vector<int>& nums) {
        int n=nums.size(),i;
        int prod=1,result=INT_MIN;
        
        for(i=0;i<n;i++)
        {
            prod*=nums[i];
            result=max(prod,result);
            if(prod==0)
                prod=1;
        }
        
        prod=1;
        for(i=n-1;i>=0;i--)
        {
            prod*=nums[i];
            result=max(prod,result);
            if(prod==0)
                prod=1;
        }
        
        return result;
    }
};
