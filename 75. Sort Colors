class Solution {
public:
    void sortColors(vector<int>& nums) {
        int zero=0,one=0,two=0,ctr=0;
        for(int i: nums)
        {
            if(i==0)
                zero++;
            else if(i==1)
                one++;
            else
                two++;
        }
        //vector<int> result;
        while(zero)
        {
            nums[ctr++]=0;
            zero--;
        }
        while(one)
        {
            nums[ctr++]=1;
            one--;
        }
        while(two)
        {
            nums[ctr++]=2;
            two--;
        }
        //return result;
    }
};
