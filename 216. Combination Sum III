class Solution {
public:
    vector<vector<int>> res;
    void comb(vector<int> com, int start, int k, int n)
    {
        if(com.size()==k && n==0)
        {
            res.push_back(com);
            return;
        }
        
        for(int i=start; i<=9; i++)
        {
            com.push_back(i);
            comb(com, i+1, k, n-i);
            com.pop_back();
        }
    }
    vector<vector<int>> combinationSum3(int k, int n) {
        
        vector<int> com;
        comb(com, 1, k, n);
        return res;
    }
};
