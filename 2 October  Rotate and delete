class Solution {
  public:
    void rotatearray(vector<int> &arr)
    {
        arr.insert(arr.begin(),arr[arr.size()-1]);
        arr.pop_back();
    }
    int rotateDelete(vector<int> &arr) {
        int n=arr.size();
        int sz=n/2;
        for(int i=1;i<=sz;i++)
        {
            rotatearray(arr);
            n=arr.size();
            arr.erase(arr.begin()+(n-i));
        }
        return arr[0];
    }
};
