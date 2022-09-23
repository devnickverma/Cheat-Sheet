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
#### 5. Non-Negative Product
```cpp
#include<bits/stdc++.h>
#define ll long long
#define int ll
using namespace std;

int32_t main()
{
    int t,n,x;
    cin >> t ;
    while(t--) {
        cin >> n;
        bool flag = false;
        int count = 0;
        for(int i=0; i<n; i++) {
            cin >> x ;
            if(x<0) {
                count++;
            }
            if(x==0) {
                flag = true;
            }
        }
        if(flag) {
            cout << 0 << endl;
        }
        else if (count%2==0) {
            cout << 0 << endl;
        }
        else {
            cout << 1 << endl;
        }
    }
    return 0;
}

```
#### 6. Two Different Palindromes
```cpp
#include<iostream>
using namespace std;

int main()
{
    int t,x,y;
    cin >> t;
    while(t--) {
        cin >> x >> y;
        if( (x%2!=0) && (y%2!=0) ) {
            cout << "NO" << endl;
        }
        else if ( (x==1) || (y==1) ) {
            cout << "NO" << endl;
        }
        else {
            cout << "YES" << endl;
        }
    }
}
```
#### 7. Even Splits
```cpp
#include<bits/stdc++.h>
#define ll long long
#define int ll
using namespace std;

int32_t main()
{
    int t,n;
    cin >> t;
    while(t--) {
        cin >> n;
        string s;
        cin >> s;
        if((s[0]=='1') && (s[1]=='0') && s.size()==2) {
            cout << s << endl;
        }
        else {
            sort(s.begin(),s.end());
            cout << s << endl;
        }
    }
}
```
