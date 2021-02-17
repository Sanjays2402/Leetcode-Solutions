class Solution {
public:
    int maxArea(vector<int>& height) {
        
        int maxi = 0, n = height.size(), i = 0, j = n-1;
        while(i < j)
        {
            int val = min(height[i], height[j]);
            maxi = max(maxi, val * (j-i));
            while(val >= height[i] && i<j)
                i++;
            while(val >= height[j] && i<j)
                j--;
        }
        return maxi;
    }
};
