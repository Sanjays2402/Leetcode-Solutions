class Solution {
public:
    static bool comp(const pair<int, int> &a, const pair<int, int> &b)
    {
        if(a.second == b.second)
            return a.first < b.first;
        return a.second < b.second;
    }
    vector<int> kWeakestRows(vector<vector<int>>& mat, int k) {
        
        vector<int> res;
        unordered_map<int, int> hash;
        for(int i=0; i<mat.size(); i++)
            for(int j=0; j<mat[i].size(); j++)
                hash[i] += mat[i][j];
        
        vector<pair<int, int>> p;
        for(auto it: hash)
            p.push_back({it.first, it.second});
        
        sort(p.begin(), p.end(), comp);
        
        for(int i=0; i<k; i++)
            res.push_back(p[i].first);
        
        return res;
    }
};
