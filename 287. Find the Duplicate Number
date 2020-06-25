class Solution {
public:
    int findDuplicate(vector<int>& nums) {
        
        map<int,int> n;
        for(int i=0;i<nums.size();i++)
        {
            if(n[nums[i]]==1)
                return nums[i];
            n[nums[i]]++;
        }
        return 0;
    }
};
