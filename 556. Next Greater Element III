class Solution {
public:
    int nextGreaterElement(int n) {
        
        if(n > INT_MAX)
            return -1;
        
        string s = "";
        int t = n;
        while(t)
        {
            s += (t%10) + '0';
            t /= 10;
        }
        
        sort(s.begin(), s.end());
        cout<<s;
        do
        {
            if(stoll(s) > n && stoll(s) <= INT_MAX)
                return stoll(s);
        }while (next_permutation(s.begin(), s.end()));
            
        return -1;
    }
};
