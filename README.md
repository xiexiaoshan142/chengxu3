# chengxu3
#include<iostream>
#include<fstream>
using namespace std;
void arraysum(int n,int left,int right)
{ int *a,sum=0,i;
  a=new int[n];
  ifstream open("D:/shuju.txt");
  for(i=0;i<n;i++)
     open>>a[i];
  for(i=0;i<n;i++)
     cout<<a[i]<<endl;
  for(i=0;i<n;i++)
     if(a[i]>=left&&a[i]<=right)
         sum+=a[i];
     cout<<n<<"个实数的总和为:"<<sum;
  open.close();
  cin.get();
}
void main()
{ int n;
  cin>>n;
  double min,max;
  cout<<"最小值为:"<<endl;
  cin>>min;
  cout<<"最大值为:"<<endl;
  cin>>max;
  Arraysum(n,min,max);
}
    
  

