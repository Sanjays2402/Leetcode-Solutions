class Solution {
public:
    vector<int> plusOne(vector<int>& digits) {
        if(digits.size()<2)
        {
            digits.back()++;
            if(digits.back()==10)
            {
                digits.back()=0;
                digits.insert(digits.begin(), 1);
            }
            return digits;
        }
        digits.back()++;
        if(digits.back() == 10)
        {
            digits.back()=0;
            for(int i=digits.size()-2; i>=0 ;i--)
            {
                digits[i]++;
                if(digits[i] != 10)
                    break;  
                if(digits.front()==10)
                {
                    digits.front()=0;
                    digits.insert(digits.begin(), 1);
                }
                else
                    digits[i]=0;
            }
        }
        return digits;
    }
};
