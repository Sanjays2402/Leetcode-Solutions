class Solution {
public:
    int shortestPathBinaryMatrix(vector<vector<int>>& grid) {
        
        int m = grid.size(), n = grid[0].size(), level = 1;
        vector<vector<bool>> visit(m, vector(n, false));
        
        if(grid[0][0] == 1 || grid[m-1][n-1] == 1)
            return -1;
        
        int dx[8] = {0, 0, 1, -1, 1, -1, 1, -1};
        int dy[8] = {1, -1, 0, 0, 1, -1, -1, 1};
        queue<pair<int, int>> q;
        visit[0][0] = true;
        q.push({0, 0});
        
        while(q.size())
        {
            int lim = q.size();
            for(int i=0; i<lim; i++)
            {
                int x = q.front().first, y = q.front().second;
                if(x == m-1 && y == n-1)
                    return level;
                q.pop();
                for(int j=0; j<8; j++)
                {
                    int o = x + dx[j];
                    int p = y + dy[j];
                    if(o >= 0 && p >= 0 && o < m && p < n && grid[o][p] == 0 && visit[o][p] == 0)
                    {
                        q.push({o, p});
                        visit[o][p] = true;
                    }
                }
            }
            level ++;
        }
        
        return -1;
    }
};
