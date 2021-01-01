class Solution {
public:
    bool canFormArray(vector<int>& arr, vector<vector<int>>& pieces) {
        
        unordered_map<int, int> hash;
        for(int i=0; i<pieces.size(); i++)
        {
            hash[pieces[i][0]] = i+1;
        }
        
        for(int i=0; i<arr.size(); )
        {
            if(hash[arr[i]])
            {
                int loc = hash[arr[i]] - 1, j=0;
                while(j < pieces[loc].size())
                {
                    if(arr[i+j] != pieces[loc][j])
                        return false;
                    j++;
                }
                i += pieces[loc].size();
            }
            else
                return false;
        }
        return true;
    }
};
