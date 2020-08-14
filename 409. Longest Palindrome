class Solution {
public:
    int longestPalindrome(string s) {
        
        unordered_map<char, int> hash;
        int count=0,first=1;
        for(char a: s)
            hash[a]++;
        for(char a: s)
        {
            if(hash[a]%2==0)
            {
                count += hash[a];
                hash[a]=0;
            }
            else if(hash[a]%2 && first)
            {
                count += hash[a];
                hash[a]=0,first=0;
            }
            else
            {
                count += hash[a]-1;
                hash[a]=0;
            }
        }
        return count;
    }
};
