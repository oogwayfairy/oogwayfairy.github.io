## 第壹題 讀入整數反序列印
#include <stdio.h>
int main()
{
	int a[1000];
	int n=0;
	
	for(int i=0; i<1000; i++){
		scanf("%d",&a[i]);
		
		if( a[i]==0 ){
			n=i;
			break;
		}
	}
	
	for(int i=n-1; i>=0; i--){
		printf("%d ",a[i]);
	}
	printf("\n");
}
## 第貳題 A的B次方函數 
'''c++
#include <stdio.h>
int MYPOWER(int a,int b)
{
	int ans=1;
	for(int i=1; i<=b; i++){
		ans=ans*a;
	}
	return ans;
}
int main(void)
{
	int a,b;
	scanf("%d%d",&a,&b);
	printf("[%d]",MYPOWER(a,b));
	return 0;
}
'''
## 第叁題 漸增數列相加
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	
	int ans=0;
	int r=0;
	
	for(int i=1; i<=n; i++){
		r=(i-1)*i;
		ans=ans+r;
	}
	printf("%d\n",ans);
}
## 第肆題 判別正方形
#include <stdio.h>
int main()
{
	int a,b;
	scanf("%d %d",&a,&b);
	
	printf("Enter two numbers: ");
	
	if(a==b)printf(" It is a square ");
	else printf(" It is not a square ");
}
## 第伍題 2進位轉10進位
#include <stdio.h>
int main()
{
	int a;
	scanf("%d",&a);
	

	printf("%d\n",a/1000*8+a%1000/100*4+a%100/10*2+a%10);
}
## 第陸題 均標與前標計算
#include <stdio.h>
int main()
{
	int n;
	float sum=0;
	int a[1000];
	scanf("%d",&n);
	
	for(int i=0; i<n; i++){
		scanf("%d",&a[i]);
	}
	
	for(int i=0; i<n; i++){
		sum=sum+a[i];
	}
	
	printf("均標:%.1f\n",sum/n);
	
	
	int h=0;
	float avg=0;
	
	for(int i=0; i<n; i++){
		if(a[i]>=sum/n){
		avg=avg+a[i];
		h++;
		}
	}
	printf("前標:%.1f\n",avg/h);
}	

