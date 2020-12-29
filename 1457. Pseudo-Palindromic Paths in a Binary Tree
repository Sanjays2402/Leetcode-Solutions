/**
 * Definition for a binary tree node.
 * struct TreeNode {
 *     int val;
 *     TreeNode *left;
 *     TreeNode *right;
 *     TreeNode() : val(0), left(nullptr), right(nullptr) {}
 *     TreeNode(int x) : val(x), left(nullptr), right(nullptr) {}
 *     TreeNode(int x, TreeNode *left, TreeNode *right) : val(x), left(left), right(right) {}
 * };
 */
class Solution {
public:
    int count = 0;
    int check(vector<int> s)
    {
        int flag = 1;
        unordered_map<int, int> hash;
        for(int i: s)
            hash[i]++;
        
        for(auto it: hash)
        {
            if( (it.second) % 2 == 1)
            {
                if(flag)
                    flag--;
                else
                    return 0;
            }
        }
        return 1;
    }
    
    void call(TreeNode* root, vector<int> s)
    {
        if(root == NULL)
        {
            if(check(s))
                count ++;
            return;
        }
        s.push_back(root->val);
        if(root->left == NULL)
            call(root->right, s);
        
        else if(root->right == NULL)
            call(root->left, s);
        
        else
        {
            call(root->right, s);
            call(root->left, s);
        }
    }
    int pseudoPalindromicPaths (TreeNode* root) {
        
        if(root == NULL)
            return 0;
        
        vector<int> s;
        call(root, s);
        
        return count;
    }
};
