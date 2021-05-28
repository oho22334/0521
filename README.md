# 0521
# 進階題：求11 +22+33+…+nn
```C
#include <stdio.h>
int main ()
{
	int n,i,sum=0;
	scanf("%d",&n);
	for(i=1;i<=n;i++){
		sum+=i*10+i;
	}
	printf("%d",sum);
}
```
# 進階題：求兩數之最大公因數
```C
#include<iostream>
using namespace std;
int GCD(int a, int b){
  int m,ans=1,i;
  if(a>b)m=a;
  else m=b;
  for(i=2;i<=m;i++)
  {
  	if(a%i==0 && b%i==0)ans=i;
  }
  return ans;  
}
int main(){
  int a,b;cin>>a>>b;
  cout<<GCD(a,b)<<endl;
  return 0;
}
```
# 進階題：區間測速-超速之王 
```C
#include <stdio.h>
int main()
{
	int i,a,min,index=1;
	scanf("%d",&min);
	for(i=2;i<=10;i++)
	{
		scanf("%d",&a);
		if(min>a)
		{
			min=a;
			index=i;
		}
	}
	int s=60*60*1.2/min;
	printf("%d %d",index,s);
	}
  ```
  # SOIT108_Advance_008：進階題：10數排序，從大到小排好 
  ```C
  #include<stdio.h>
int main()
{
	int a[10],i,j,temp;
	for(i=0;i<10;i++)
	{
		scanf("%d",&a[i]);
	 
	 }
	 for(i=0;i<10;i++)
	 {
	 	for(j=i;j<10;j++)
	 	{
	 		if(a[i]<a[j])
	 		{
	 			temp=a[i];
	 			a[i]=a[j];
	 			a[j]=temp;
	 		}
	 	}
	 }
	 for(i=0;i<10;i++)
	 {
	 	printf("%d ",a[i]);
	 }
}
```
