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
    int sum = 0;
    int len(TreeNode* root)
    {
        if(root == NULL)
            return 0;
        return max(len(root->left), len(root->right)) + 1;
    }
    void traverse(TreeNode* root, int cur, int height)
    {
        if(root == NULL)
            return;
        if(cur == height)
        {
            sum += root->val;
            return;
        }
        traverse(root->left, cur+1, height);
        traverse(root->right, cur+1, height);
        
        return;
    }
    int deepestLeavesSum(TreeNode* root) {
        
        int dept = len(root);
        traverse(root, 1, dept);
        
        return sum;
    }
};
