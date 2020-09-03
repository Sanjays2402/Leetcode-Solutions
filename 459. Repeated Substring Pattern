class Solution {
public:
    bool repeatedSubstringPattern(string s) {
        int len=1;
        while(len<=s.length()/2)
        {
            if(s.length()%len==0)
            {
                string a=s.substr(0,len);
                int flag=1;
                for(int i=len; i<s.length(); i+=len)
                {
                    if(a != s.substr(i, len))
                    {
                        flag=0;
                        break;
                    }
                }
                if(flag)
                    return true;
            }
            len++;
        }
        return false;
    }
};
