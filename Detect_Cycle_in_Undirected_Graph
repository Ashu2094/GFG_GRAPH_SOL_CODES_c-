class Solution {
  public:
  bool ans=false;
  void dfs (int vertex,int V,vector<int> adj[],vector <bool> &visited,vector <bool> &inStack)
  {
      visited[vertex]=true;
      inStack[vertex]=true;
      for(auto x:adj[vertex])
      {
          if(inStack[x])
          ans=true;
          if(!visited[x])
          {
              dfs(x,V,adj,visited,inStack);
          }
      }
      inStack[vertex]=false;
  }
   
   
   
    bool isCyclic(int V, vector<int> adj[]) {
        // code here
        
        vector <bool> visited(V,0);
        vector <bool> inStack(V,0);
        for(int i=0;i<V;i++)
        {
            if(!visited[i])
            dfs(i,V,adj,visited,inStack);
        }
        
        return ans;
    }
};
