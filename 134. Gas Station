class Solution {
public:
    int canCompleteCircuit(vector<int>& gas, vector<int>& cost) {
        
        int sum=0, start=0, end=gas.size(), counter=0, i=0;
        while(start < end)
        {
            if(sum >= 0)
            {
                sum += gas[start] - cost[start];
            }
            else
            {
                i=start;
                counter += sum;
                sum = 0;
                sum += gas[start] - cost[start];
            }
            start++;
        }
        if(sum+counter >= 0)
            return i;
        return -1;
    }
};
