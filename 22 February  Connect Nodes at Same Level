class Solution{
    public:
     void connect(Node *root)
    {
       vector<Node*> store;
       queue<Node*> array;
       array.push(root);
       array.push(NULL);
       while(!array.empty())
       {
           Node *front = array.front();
           array.pop();
           if(store.size() != 0)
           {
               store[store.size()-1]->nextRight = front;
           }
           store.push_back(front);
           if(front->left != NULL)
           {
               array.push(front->left);
           }
           if(front->right != NULL)
           {
               array.push(front->right);
           }
           if(array.front() == NULL)
           {
               array.pop();
               store.clear();
               if(!array.empty())
               {
                 array.push(NULL);
               }
           }
       }
    }   
};
