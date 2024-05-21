class Solution {
  public:
    vector<int> printKClosest(vector<int> arr, int n, int k, int x) {
        map<int,vector<int>> mp;
        for(auto it:arr){
            mp[abs(it-x)].push_back(it);
        }
        vector<int> ans;
        for(auto it:mp){
            if(it.first==0){
                continue;
            }
            if(k==0){
                break;
            }
            sort(it.second.rbegin(),it.second.rend());
            for(auto num:it.second){
                ans.push_back(num);
                k--;
                if(k==0){
                    break;
                }
            }
        }
        return ans;
    }
};
