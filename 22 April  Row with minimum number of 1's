class Solution {
  public:
    int minRow(int n, int m, vector<vector<int>> a) {
        int ans = INT_MAX, count, val;
        for(int i=0; i<n; i++){
            count = 0;
            for(int j=0; j<m; j++){
                if(a[i][j]==1) count++; 
            }
            if(count < ans){
                ans = count;
                val = i+1;
            }
        }
        return val;
    }
};
