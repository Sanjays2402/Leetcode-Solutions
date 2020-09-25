class Solution {
public:
    bool comp(int a, int b)
    {
        string aa=to_string(a);
        string bb=to_string(b);
        return bb+aa > aa+bb;
    }
    string largestNumber(vector<int>& nums) {
        
        string result = "";
        for(int i=0; i<nums.size()-1; i++)
        {
            for(int j=i+1; j<nums.size(); j++)
            {
                if(comp(nums[i], nums[j]))
                    swap(nums[i], nums[j]);
            }
        }
        for(int i: nums)
            result += to_string(i);
        
        while(result[0]=='0' && result.length()>1)
            result.erase(0,1);
        
        return result;
    }
};
