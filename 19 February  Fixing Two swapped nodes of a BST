class Solution {
  public:
    Node *prev = NULL, *first = NULL, *second;
    void fix (Node *root) {
        if (root == NULL) return;
        fix (root->left);
        if (prev != NULL && root->data < prev->data) {
            if (first == NULL)
                first = prev;
            second = root;
        }
        prev = root;
        fix (root->right);
    }
   
    struct Node *correctBST(struct Node *root) {
        fix (root);
        swap (first->data, second->data);
        return root;
    }
};
