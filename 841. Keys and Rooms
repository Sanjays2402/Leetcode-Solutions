class Solution {
public:
    bool canVisitAllRooms(vector<vector<int>>& rooms) {
        
        int n = rooms.size();
        set<int> st;
        queue<int> q;
        vector<int> visit(n, -1);
        q.push(0);
        
        while(q.size())
        {
            int t = q.size();
            for(int i=0; i<t; i++)
            {
                int cur = q.front();
                q.pop();
                st.insert(cur);
                
                if(visit[cur] == 1)
                    continue;
                
                for(int j=0; j<rooms[cur].size(); j++)
                    q.push(rooms[cur][j]);
                
                visit[cur] = 1;
            }
        }
        
        return st.size() == n;
    }
};
