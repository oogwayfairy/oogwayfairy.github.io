# oogwayfairy.github.io

## My first personal website !

## 第2次作業
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

## activity
  
![寶可夢]https://img.3dmgame.com/uploads/images/news/20191206/1575624597_738576.jpg
