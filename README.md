# 24IBD70007-exp2.2.2-groupB-shubham-sharma-cc
class Solution {
public:
    TreeNode* inorderSuccessor(TreeNode* root, TreeNode* p) {
        TreeNode* successor = NULL;

        while (root) {
            if (p->val < root->val) {
                successor = root;
                root = root->left;
            } else {
                root = root->right;
            }
        }

        return successor;
    }
};
