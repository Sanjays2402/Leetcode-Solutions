class Solution {
public:
    vector<int> findDiagonalOrder(vector<vector<int>>& matrix) {
        
        int m = matrix.size();
        if(m == 0)
            return {};
        
        int n = matrix[0].size();
        vector<int> res;
        map<int, vector<int>> hash;
        
        for(int i=0; i<matrix.size(); i++)
        {
            for(int j=0; j<matrix[0].size(); j++)
            {
                hash[i+j].push_back(matrix[i][j]);
            }
        }
        
        for(int i=0; i<m+n-1; i++)
        {
            if(i%2 == 0)
                reverse(hash[i].begin(), hash[i].end());
            for(int j: hash[i])
                    res.push_back(j);
        }
        
        return res;
    }
};
