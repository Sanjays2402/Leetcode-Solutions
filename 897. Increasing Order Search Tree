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
    TreeNode* res = new TreeNode();
    
    void inorder(TreeNode* root)
    {
        if(root == NULL)
            return;
        
        inorder(root->left);
        {
            res->right = new TreeNode(root->val);
            res = res->right;
        }
        inorder(root->right);
    }
    TreeNode* increasingBST(TreeNode* root) {
        
        TreeNode* temp = res;
        inorder(root);
        return temp->right;
    }
};
