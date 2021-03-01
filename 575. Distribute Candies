class Solution {
public:
    int distributeCandies(vector<int>& candyType) {
        
        int n = candyType.size();
        set<int> s;
        for(int i: candyType)
            s.insert(i);
        
        int len = s.size();
        return min(len, n/2);
    }
};
