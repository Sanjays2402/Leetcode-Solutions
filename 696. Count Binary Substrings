class Solution {
public:
    int countBinarySubstrings(string s) {
        
        int count = 0, cur = 1, pre = 0;
        
        for(int i=1; i<s.size(); i++)
        {
            if(s[i] == s[i-1])
                cur++;
            else
            {
                count += min(cur, pre);
                pre = cur;
                cur = 1;
            }
        }
        return count + min(cur, pre);
    }
};
