class Solution {
public:
    int twoCitySchedCost(vector<vector<int>>& costs) {
        
        int m=costs.size(),sum=0;
        
        sort( costs.begin(), costs.end() , [](vector<int> &a , vector<int> &b)
             {
                 if(a[0]-a[1] > b[0]-b[1])
                    return true;
                 return false;
             });
        
        for(int i=0 ; i<costs.size()/2 ; i++)
            sum += costs[i][1];
        
        for(int i=costs.size()/2 ; i<costs.size() ; i++)
            sum += costs[i][0];
        
        return sum;
    } 
};
