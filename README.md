# wave

//To print wave by 2D matrix
#include <iostream>
using namespace std;
int printwave(int a[][3], int n, int row,int col){
    while(n!=0)
    {
        int i;
        if(col&1){
        //odd column
        for(int row=n-1;row<=0;row--){
            cout<<a[row][col]<<" ";
        }
           }
         else{
        //even column
        for(int row=0;row<n-1;row++){
            cout<<a[row][col]<<" ";
        }
            }
    }
}

int main() {
    int n,a[3][3],i,j;
   cout<<"enter elements of the aray";
    for( i=0;i<3;i++){
        for( j=0;j<3;j++){
            cin>>a[i][j];
        }
        cout<<endl;
    }
    cout<<"wave:";
    cout<<a[i][j]<<printwave(a,n,i,j);
  
    return 0;
}
