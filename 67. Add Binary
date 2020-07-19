class Solution {
public:
    string addBinary(string a, string b) {
        
        string result="";
        int i=a.size()-1, j=b.size()-1,plus=0;
        
        while(i>=0 && j>=0)
        {
            if(a[i]=='1' && b[j]=='1')
            {
                if(plus==1)
                    result += "1";
                else
                    result += "0";
                plus = 1;
            }
            else if(a[i]=='1' || b[j]=='1')
            {
                if(plus==1)
                    result += "0",plus=1;
                else
                    result += "1",plus=0;
            }
            else
            {
                if(plus==1)
                    result += "1";
                else
                    result += "0";
                plus=0;
            }
            i--,j--;
        }
        while(i>=0)
        {
            if(a[i]=='1')
            {
                if(plus==1)
                    result += "0",plus=1;
                else
                    result += "1",plus=0;
            }
            else
            {
                if(plus==1)
                    result += "1";
                else
                    result += "0";
                plus=0;
            }     
            i--;
        }
        while(j>=0)
        {
            if(b[j]=='1')
            {
                if(plus==1)
                    result += "0",plus=1;
                else
                    result += "1",plus=0;
            }
            else
            {
                if(plus==1)
                    result += "1";
                else
                    result += "0";
                plus=0;
            } 
            j--;
        }
        if(plus==1)
            result += "1";
        reverse(result.begin(), result.end());
        return result;
    }
};
