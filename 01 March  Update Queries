class Solution{
    public:
        vector<int> updateQuery(int n,int q,vector<vector<int>> &v)
        {
            unordered_map<int,vector<int>>mp;
            for(auto x :v){
                mp[x[0]-1].push_back(x[2]);
                mp[x[1]].push_back(-x[2]);
                
            }
            vector<int>ans(n,0);
            map<int,int>temp;
            for(int i =0;i<n;i++){
                if(mp.find(i)!=mp.end()){
                    for(auto x:mp[i]){
                        if(x<0){
                            temp[-x]--;;
                        }
                        else {
                            temp[x]++;
                        }
                    }
                }
                int res =0;
                for(auto x :temp){
                    if(x.second>0)
                    res=res|x.first;
                }
                ans[i]=res;
            }
            return ans;
        }
};
