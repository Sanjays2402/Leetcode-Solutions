class Solution {
public:
    int islandPerimeter(vector<vector<int>>& grid) {
        
        int m=grid.size(), n=grid[0].size();
        int count=0;
        
        for(int i=0; i<m; i++)
        {
            for(int j=0; j<n; j++)
            {
                if(grid[i][j]==1)
                {
                    if(i==0 || !grid[i-1][j])
                        count++;
                    if(j==0 || !grid[i][j-1])
                        count++;
                    if(i==m-1 || !grid[i+1][j])
                        count++;
                    if(j==n-1 || !grid[i][j+1])
                        count++;
                    
                }
            }
        }
        
        return count;
    }
};
