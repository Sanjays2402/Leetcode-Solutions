class Solution {
public:
    string reverseWords(string s) {
        
        int i,j,start=0;
        while(s[i]==' ')
            s.erase(s.begin()+i);
        reverse(s.begin(), s.end());
        while(s[i]==' ')
            s.erase(s.begin()+i);
        
        for(i=0; i<s.length(); i++)
        {
            if(s[i]==' ')
            {
                reverse(s.begin()+start, s.begin()+i);
                start=i+1;
            }
            else if(i==s.length()-1)
                reverse(s.begin()+start, s.begin()+i+1);
            
            while(s[i]==' ' && s[i+1]==' ')
                s.erase(s.begin()+i);
                
        }
        return s;
    }
};
