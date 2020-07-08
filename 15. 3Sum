class Solution {
public:
    vector<vector<int>> threeSum(vector<int>& nums) {
        
        vector<vector<int>> result;
        if(nums.size()<3)
            return result;
        
        sort(nums.begin(), nums.end());
        for(int i=0; i<nums.size()-2; i++)
        {
            if(nums[i]>0)
                return result;
            int left=i+1, right=nums.size()-1;
            if(i>0 && nums[i]==nums[i-1])
                continue;
            else
            {
                while(left<right)
                {
                    int sum=nums[i]+nums[left]+nums[right];
                    if(sum>0)
                        right--;
                    else if(sum<0)
                        left++;
                    else
                    {
                        int temp_left=nums[left], temp_right=nums[right];
                        result.push_back({nums[i], nums[left], nums[right]});
                        right--, left++;
                        while(left<nums.size() && nums[left]==temp_left)
                            left++;
                        while(right>i && nums[right]==temp_right)
                            right--;
                    }
                }
            }
        }
        return result;
    }
};
