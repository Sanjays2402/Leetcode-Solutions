class Solution {
public:
    int count1(vector<vector<int>> a, int x, int y)
    {
        int count = 0, m = a.size(), n = a[0].size();
        
        if(x!=0 && a[x-1][y])
            count++;
        if(x!=0 && y!=0 && a[x-1][y-1])
            count++;
        if(x!=0 && y!=n-1 && a[x-1][y+1])
            count++;
        if(y!=n-1 && a[x][y+1])
            count++;
        if(x!=m-1 && y!=n-1 && a[x+1][y+1])
            count++;
        if(x!=m-1 && a[x+1][y])
            count++;
        if(x!=m-1 && y!=0 && a[x+1][y-1])
            count++;
        if(y!=0 && a[x][y-1])
            count++;
        
        return count;
    }
    void gameOfLife(vector<vector<int>>& board) {
        
        vector<vector<int>> temp = board;
        
        for(int i=0; i<board.size(); i++)
        {
            for(int j=0; j<board[0].size(); j++)
            {
                int ct = count1(board, i, j);
                if(board[i][j])
                {
                    if(ct<2)
                        temp[i][j] = 0;
                    else if(ct == 2 || ct == 3)
                        temp[i][j] = 1;
                    else
                        temp[i][j] = 0;
                }
                else
                {
                    if(ct == 3)
                        temp[i][j] = 1;
                }
            }
        }
        
        board = temp;
    }
};
