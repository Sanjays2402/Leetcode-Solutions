class Solution {
public:
    vector<int> sequentialDigits(int low, int high) {
        
        
        vector<int> res;
        int len1=to_string(low).length(), len2=to_string(high-1).length();
        string comp="";
        for(int i=1; i<10; i++)
            comp += to_string(i);
        
        for(int i=len1; i<=len2; i++)
        {
            cout<<i<<endl;
            for(int j=0; j<=comp.length()-i; j++)
            {
                bool flag=true;
                if(i==2)
                    if(comp[j]+1 != comp[j+1])
                        flag=false;
                else
                    for(int k=j; k<j+i-1; k++)
                    {
                        if(comp[k]+1 != comp[k+1])
                        {
                            flag=false;
                            break;
                        }
                    }
                if(flag && stoll(comp.substr(j,i))>=low && stoll(comp.substr(j,i))<=high)
                    res.push_back(stoll(comp.substr(j,i)));
            }
        }
        
        return res;
    }
};
