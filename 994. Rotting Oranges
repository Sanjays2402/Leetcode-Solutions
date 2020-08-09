class Solution {
public:
    void rot(vector<vector<int>>& grid, int i, int j, int rotcount)
    {
        if(i!=0 && grid[i-1][j]==1)
            grid[i-1][j]=rotcount+1;
        if(j!=0 && grid[i][j-1]==1)
            grid[i][j-1]=rotcount+1;
        if(i!=grid.size()-1 && grid[i+1][j]==1)
            grid[i+1][j]=rotcount+1;
        if(j!=grid[0].size()-1 && grid[i][j+1]==1)
            grid[i][j+1]=rotcount+1;
    }
    
    int orangesRotting(vector<vector<int>>& grid) {
        
        int m=grid.size(), n=grid[0].size(),flag=0;
        int rotcount=2, count=0;
        for(int i=0;i<m;i++)   
            for(int j=0;j<n;j++)
                if(grid[i][j]==1)
                    flag++;
        if(!flag)
            return 0;
        while(true)
        {
            bool found=false;
            for(int i=0; i<m; i++)
            {
                for(int j=0; j<n; j++)
                {
                    if(grid[i][j]==rotcount)
                    {
                        rot(grid, i ,j, rotcount);
                        flag=true;
                    }
                }
            }
            if(flag)
                count++;
            for(int i=0; i<m; i++)
                for(int j=0; j<n; j++)
                    if(grid[i][j]==1)
                        found=true;
            if(!found)
            {    
                return count;
            }
            if(rotcount>m*n)
                return -1;
            rotcount++;
        }
        return -1;
    }
};
