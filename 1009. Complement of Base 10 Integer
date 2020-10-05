class Solution {
public:
    int bitwiseComplement(int N) {
        
        if(N == 0)
            return 1;
        int k=0, sum=0;
        while(N)
        {
            sum += (1 - (N%2)) * pow(2, k++);
            N/=2;
        }
        return sum;
    }
};
