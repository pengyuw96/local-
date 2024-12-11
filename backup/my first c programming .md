#include <stdio.h>
int main(){
    int M,N;
    scanf("%d %d",&M,&N);
    if(M>N ||M<100|| N>999){
        printf("Invalid Value.");
    }
    else{
        for(int i=M;i<=N;i++){
            int t=i,sum=0;
            while(t){
            sum+=(t%10)*(t%10)*(t%10);
            t/=10;
            }
            if(sum==i){
                printf("%d\n",i);}
        }
    }
    return 0;
}