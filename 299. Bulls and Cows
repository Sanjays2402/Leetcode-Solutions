class Solution {
public:
    string getHint(string secret, string guess) {
        
        int count=0;
        string res="";
        for(int i=0; i<secret.length(); i++)
            if(secret[i] == guess[i])
            {
                count++;
                secret[i]='*';
                guess[i]='*';
            }
        
        res += to_string(count);
        res += 'A';
        count=0;
        
        map<char, int> hash;
        for(char i: secret)
            hash[i]++;
        
        for(char i: guess)
        {
            if(hash[i] && i!='*')
            {    
                count++;
                hash[i]--;
            }
        }
        res += to_string(count);
        res += 'B';
        return res;
    }
};
