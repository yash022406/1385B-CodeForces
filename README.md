# 1385B-CodeForces
#include <iostream>
using namespace std;
int main() {
    int n;
    cin>>n;
    while(n--){
        int t,i,j;
        cin>>t;
        int a[2*t];
        for(i=0;i<2*t;i++){
            cin>>a[i];
        }
        for(i=0;i<2*t;i++){
            if(a[i]!=0){
                for(j=i+1;j<2*t;j++){
                    if(a[j]==a[i]){
                        a[j]=0;
                    }
                }
            }
        
            
        }
        for(i=0;i<2*t;i++){
            if(a[i]!=0){
                cout<<a[i]<<" ";
            }
        }
        cout<<endl;
    }

    return 0;
}
