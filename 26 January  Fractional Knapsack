class Solution
{
    public:
    static bool comp(Item a, Item b)
    {
        return ((1.0 * a.value)/(a.weight*1.0))>((1.0*b.value)/(b.weight*1.0));
    }
    double fractionalKnapsack(int W, Item arr[], int n)
    {
        sort(arr,arr+n,comp);
        double ans=0;
        for (int i=0;i<n;i++)
        {
            if (W>=arr[i].weight) 
            {
                ans+=arr[i].value;
                W-=arr[i].weight;
            }
            else
            {
                ans+=arr[i].value*((1.0*W)/(1.0*arr[i].weight));
                break;
            }
        }
        return ans;
    }
        
};
