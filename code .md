     #include<bits/stdc++.h>
    #define ll   long long 
    #define ff first
    #define ss second
    #define pb push_back
    #define pf push_front
    #define vec vector 
    #define min_heap priority_queue <ll, vector<ll>, greater<ll> >
    #define present(container, element)(container.find(element) != container.end())
    #define cpresent(container, element)(find(all(container), element) != container.end())
    #define all(v) v.begin(),v.end()
    #define allr(v) v.rbegin(),v.rend()
    #define gcd(a,b) __gcd(a,b)
    #define     max3(a,b,c)     max(a,max(b,c))
    #define     max4(a,b,c,d)   max(max3(a,b,c),d)
    #define     min3(a,b,c)     min(a,min(b,c))
    #define     min4(a,b,c,d)   min(a,min3(b,c,d))
    #define er cout<<-1<<endl;
    #define  fast ios_base::sync_with_stdio(false);cin.tie(NULL);
    #define  mod 1000000007// 1e9+7
    #define pi 3.1415926536
    #define REP(i,a,b) for (int i = a; i <= b; i++)
    using namespace std;
    //debbug
    template < typename F, typename S >
    ostream& operator << ( ostream& os, const pair< F, S > & p ) {
                return os << "(" << p.first << ", " << p.second << ")";
    }
     
    template < typename T >
    ostream &operator << ( ostream & os, const vector< T > &v ) {
                os << "{";
                    for(auto it = v.begin(); it != v.end(); ++it) {
                                    if( it != v.begin() ) os << ", ";
                                            os << *it;
                                                }
                        return os << "}";
    }
     
    template < typename T >
    ostream &operator << ( ostream & os, const set< T > &v ) {
                os << "[";
                    for(auto it = v.begin(); it != v.end(); ++it) {
                                    if( it != v.begin() ) os << ", ";
                                            os << *it;
                                                }
                        return os << "]";
    }
     
    template < typename T >
    ostream &operator << ( ostream & os, const multiset< T > &v ) {
                os << "[";
                    for(auto it = v.begin(); it != v.end(); ++it) {
                                    if( it != v.begin() ) os << ", ";
                                            os << *it;
                                                }
                        return os << "]";
    }
     
    template < typename F, typename S >
    ostream &operator << ( ostream & os, const map< F, S > &v ) {
                os << "[";
                    for(auto it = v.begin(); it != v.end(); ++it) {
                                    if( it != v.begin() ) os << ", ";
                                            os << it -> first << " = " << it -> second ;
                                                }
                        return os << "]";
    }
     
    #define dbg(args...) do {cerr << #args << " : "; faltu(args); } while(0)
     
    void faltu () {
                cerr << endl;
    }
     
    template <typename T>
    void faltu( T a[], int n ) {
                for(int i = 0; i < n; ++i) cerr << a[i] << ' ';
                    cerr << endl;
    }
     
    template <typename T, typename ... hello>
    void faltu( T arg, const hello &... rest) {
                cerr << arg << ' ';
                    faltu(rest...);
    }//debug

  ll lcm(ll a,ll b)
    {
        return (a*b)/gcd(a,b);

    }

      
    void no()
    {
        cout<<"NO"<<endl;
    }
    void yes()
    {
        cout<<"YES"<<endl;
     
     
    }
   ll powerOfTwo(ll n)
    {
        return n && (!(n & (n-1)));
    }
    

    

      
    void solve()
    {
       

       int n;

       cin>>n;
      int a[n+5];
      for(int i=1;i<=n;i++)cin>>a[i];
      sort(a+1,a+n+1);
      if(n%2==1)
      {

          int x=a[n/2+1];
          int  sum=0;
             for(int i=1;i<=n;i++){
sum+=min(abs(x-a[i]),abs(a[i]-1));


             }
             cout<<x<<' '<<sum<<endl;
return;



      }
      int sum1=0;
      int sum2=0;

         if(n%2==0)
      {

          int x=a[n/2];
          sum1=0;
             for(int i=1;i<=n;i++){
sum1+=abs(x-a[i]);


             }

             

      }
          if(n%2==0)
      {

          int x=a[n/2+1];
          sum2=0;
             for(int i=1;i<=n;i++){
sum2+=abs(x-a[i]);


             }

             

      }
      if(sum1<sum2)
     {
         cout<<a[n/2]<<' '<<sum1<<endl;
     }
     else   
     {
         cout<<a[n/2+1]<<' '<<sum2<<endl;
     }     
      










    }

     
    int  main()
    {
     

solve();


     
     
    return 0;
     
    }     #include<bits/stdc++.h>
    #define ll   long long 
    #define ff first
    #define ss second
    #define pb push_back
    #define pf push_front
    #define vec vector 
    #define min_heap priority_queue <ll, vector<ll>, greater<ll> >
    #define present(container, element)(container.find(element) != container.end())
    #define cpresent(container, element)(find(all(container), element) != container.end())
    #define all(v) v.begin(),v.end()
    #define allr(v) v.rbegin(),v.rend()
    #define gcd(a,b) __gcd(a,b)
    #define     max3(a,b,c)     max(a,max(b,c))
    #define     max4(a,b,c,d)   max(max3(a,b,c),d)
    #define     min3(a,b,c)     min(a,min(b,c))
    #define     min4(a,b,c,d)   min(a,min3(b,c,d))
    #define er cout<<-1<<endl;
    #define  fast ios_base::sync_with_stdio(false);cin.tie(NULL);
    #define  mod 1000000007// 1e9+7
    #define pi 3.1415926536
    #define REP(i,a,b) for (int i = a; i <= b; i++)
    using namespace std;
    //debbug
    template < typename F, typename S >
    ostream& operator << ( ostream& os, const pair< F, S > & p ) {
                return os << "(" << p.first << ", " << p.second << ")";
    }
     
    template < typename T >
    ostream &operator << ( ostream & os, const vector< T > &v ) {
                os << "{";
                    for(auto it = v.begin(); it != v.end(); ++it) {
                                    if( it != v.begin() ) os << ", ";
                                            os << *it;
                                                }
                        return os << "}";
    }
     
    template < typename T >
    ostream &operator << ( ostream & os, const set< T > &v ) {
                os << "[";
                    for(auto it = v.begin(); it != v.end(); ++it) {
                                    if( it != v.begin() ) os << ", ";
                                            os << *it;
                                                }
                        return os << "]";
    }
     
    template < typename T >
    ostream &operator << ( ostream & os, const multiset< T > &v ) {
                os << "[";
                    for(auto it = v.begin(); it != v.end(); ++it) {
                                    if( it != v.begin() ) os << ", ";
                                            os << *it;
                                                }
                        return os << "]";
    }
     
    template < typename F, typename S >
    ostream &operator << ( ostream & os, const map< F, S > &v ) {
                os << "[";
                    for(auto it = v.begin(); it != v.end(); ++it) {
                                    if( it != v.begin() ) os << ", ";
                                            os << it -> first << " = " << it -> second ;
                                                }
                        return os << "]";
    }
     
    #define dbg(args...) do {cerr << #args << " : "; faltu(args); } while(0)
     
    void faltu () {
                cerr << endl;
    }
     
    template <typename T>
    void faltu( T a[], int n ) {
                for(int i = 0; i < n; ++i) cerr << a[i] << ' ';
                    cerr << endl;
    }
     
    template <typename T, typename ... hello>
    void faltu( T arg, const hello &... rest) {
                cerr << arg << ' ';
                    faltu(rest...);
    }//debug

  ll lcm(ll a,ll b)
    {
        return (a*b)/gcd(a,b);

    }

      
    void no()
    {
        cout<<"NO"<<endl;
    }
    void yes()
    {
        cout<<"YES"<<endl;
     
     
    }
   ll powerOfTwo(ll n)
    {
        return n && (!(n & (n-1)));
    }
    

    

      
    void solve()
    {
       

       int n;

       cin>>n;
      int a[n+5];
      for(int i=1;i<=n;i++)cin>>a[i];
      sort(a+1,a+n+1);
      if(n%2==1)
      {

          int x=a[n/2+1];
          int  sum=0;
             for(int i=1;i<=n;i++){
sum+=min(abs(x-a[i]),abs(a[i]-1));


             }
             cout<<x<<' '<<sum<<endl;
return;



      }
      int sum1=0;
      int sum2=0;

         if(n%2==0)
      {

          int x=a[n/2];
          sum1=0;
             for(int i=1;i<=n;i++){
sum1+=abs(x-a[i]);


             }

             

      }
          if(n%2==0)
      {

          int x=a[n/2+1];
          sum2=0;
             for(int i=1;i<=n;i++){
sum2+=abs(x-a[i]);


             }

             

      }
      if(sum1<sum2)
     {
         cout<<a[n/2]<<' '<<sum1<<endl;
     }
     else   
     {
         cout<<a[n/2+1]<<' '<<sum2<<endl;
     }     
      










    }

     
    int  main()
    {
     

solve();


     
     
    return 0;
     
    }
