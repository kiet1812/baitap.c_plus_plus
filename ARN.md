``` c++
#include <bits/stdc++.h>
using namespace std;
int main(){
	ios_base::sync_with_stdio(false);
	cin.tie(0); cout.tie(0);
    freopen("arn.inp","r",stdin);
	freopen("arn.out","w",stdout);
	string str; cin>>str;
    string dem;cin>>dem;
    int s=0;
    if(str.find(dem)>1000){
        cout<<0;
        return 0;
    }
    while(str.find(dem)<=1000){
        if(str.find(dem)<=1000) s++;
        str.erase(0,str.find(dem)+1);
    }
    cout<<s;
    return 0;
}
```
