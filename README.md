# Friends-pairing-

    
public:
int mod=1000000007;
    int countFriendsPairings(int n) 
    { int dp[n+1];
dp[0]=0;
dp[1]=1;
dp[2]=2;
for(long long int i=3;i<=n;i++){
    
dp[i] = ((dp[i-1])%mod+(i-1)%mod*(dp[i-2])%mod)%mod;

}
return dp[n];
        
        
        // code here
    }
};  
