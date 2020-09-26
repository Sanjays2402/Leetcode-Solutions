class Solution {
public:
    int findPoisonedDuration(vector<int>& time, int duration) {
        
        if(time.size() == 0)
            return 0;
        int result=duration;
        for(int i=1; i<time.size(); i++)
        {
            if(time[i] < time[i-1] + duration)
            {
                result += (time[i] - time[i-1]);
            }
            else
                result += duration;
        }
        return result;
    }
};
