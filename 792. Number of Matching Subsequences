class Solution {
public:
    bool isSubsequence(string s, string t) {
        if(t.size() == 0 && s.size()==0)
            return true;
        
        int i=0, j=0;
        while(j<t.size()){
            if(s[i] == t[j])
                i++;
            if(i==s.size())
                return true;
            j++;
        }
        return false;
    }
    
    int numMatchingSubseq(string S, vector<string>& words) {
        int cnt = 0;
        unordered_map<string, int> map;
        for(string word: words)
            map[word]++;
        
        for(auto i: map){
            if(isSubsequence(i.first, S))
                cnt += i.second;
        }
        return cnt;
    }
};
