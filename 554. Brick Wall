class Solution {
public:
    int leastBricks(vector<vector<int>>& wall) {
        
        int res = 0, len=0;
        unordered_map<int, int> hash, counthash;
        for(int i=0; i<wall[0].size(); i++)
            len += wall[0][i];
        for(int i=0; i<wall.size(); i++)
        {
            for(int j=0; j<wall[i].size(); j++)
            {
                hash[i] += wall[i][j];
                counthash[hash[i]] ++;
            }
        }
        for(auto it: counthash)
        {
            if(it.first != len)
                res = max(res, it.second);
        }
        
        return wall.size() - res;
    }
};
