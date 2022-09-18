# Cheat-Sheet
CPP Cheat Sheet for CP

#### 1. 10^9 long long
#### 2. Sum of 1 to n even & odd numbers
```bash
Sum of even : (n*n)
Sum of odd : (n*(n+1))
```

#### 3. Find sum of all pair in array
```bash
Using map : ans += (i.second*(i.second - 1))/2;
```
#### 4. COOL NAME CODECHEF
```cpp
#include<bits/stdc++.h>
using namespace std;

int main()
{
    int t;
    cin >> t;
    while(t--) {
     string s; cin>>s;
     sort(s.begin(), s.end());
     int sum=0;
     for(int i=0; i<s.size(); i++){
       int pos = int(s[i])-96;
       int ans = pos*(i+1);
       sum += ans;
      }
      cout<<sum<<endl;
    }
    return 0;
}
```
