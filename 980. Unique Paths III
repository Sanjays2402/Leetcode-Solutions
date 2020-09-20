class Solution {
public:
    int dfs(vector<vector<int>> &a, int i, int j, int count)
    {
      if(i<0 || j<0 || i>=a.size() || j>=a[0].size() || a[i][j] == -1)
      {
        return 0;
      }
      if(a[i][j]==2)
          return count==-1?1:0;
      
      count--;
      a[i][j]=-1;
      int totcount = dfs(a, i+1, j, count) + dfs(a, i, j+1, count) + dfs(a, i-1, j, count) + dfs(a, i, j-1, count);
      count++;
      a[i][j]=0;
      
      return totcount;
      
      
    }
    int uniquePathsIII(vector<vector<int>>& grid) {
        
      int x,y,count=0;
      for(int i=0; i<grid.size(); i++)
      {
        for(int j=0; j<grid[0].size(); j++)
        {
          if(grid[i][j] == 0)
            count++;
          else if(grid[i][j] == 1)
          {
            x=i,y=j;
          }
        }
      }
      
      return dfs(grid, x, y, count);
    }
};
