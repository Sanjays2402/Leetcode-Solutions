class Solution {
public:
    vector<string> wordSubsets(vector<string>& A, vector<string>& B) {
        
        vector<string> res;
        vector<int> maxi(26, 0);
        
        for(int i=0; i<B.size(); i++)
        {
            vector<int> temp(26, 0);
            for(char j: B[i])
            {
                temp[j - 'a']++;
                maxi[j-'a'] = max(maxi[j-'a'], temp[j-'a']);
            }
        }
        for(int i=0; i<A.size(); i++)
        {
            int flag = 1;
            vector<int> temp(26, 0);
            for(char j: A[i])
                temp[j - 'a'] ++;
            
            for(char j='a'; j<='z'; j++)
            {
                if(maxi[j-'a'] > temp[j-'a'])
                {
                    flag = 0;
                    break;
                }
            }
            if(flag)
                res.push_back(A[i]);
        }
        return res;
    }
};
