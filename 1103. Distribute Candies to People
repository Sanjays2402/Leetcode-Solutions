class Solution {
public:
    vector<int> distributeCandies(int candies, int n) {
        
        vector<int> result(n);
        int i=0,candie=1;
        while(candies>0)
        {
            result[i++ % n] += min(candie, candies);
            candies -= candie;
            candie++;
        }
        
        return result;
    }
};
