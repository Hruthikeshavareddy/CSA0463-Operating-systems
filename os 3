#include<stdio.h>
int main()
{
	int n=0,i=0,j=0,wt[10],bt[10],tat[10];
	float avgtat,avgwt;
	printf("enter the number of processes(maximum 10):");
	scanf("%d",&n);
	printf("enter the burst time for the processes\n");
	for(i=0;i<n;i++)
	{
		printf("p%d = ",i+1);
		scanf("%d",&bt[i]);
	}
	wt[0]=0;
	for(i=1;i<n;i++)
	{
		wt[i]=0;
		for(j=0;j<i;j++)
		{
			wt[i]+=bt[j];
		}
	}
	printf("\nprocesses\tbursttime\twaitingtime\tturnaroundtime");
	for(i=0;i<n;i++)
	{
		tat[i]=wt[i]+bt[i];
		avgwt+=wt[i];
		avgtat+=tat[i];
	    printf("\nP%d\t\t%d\t\t%d\t\t%d",i+1,bt[i],wt[i],tat[i]);
	}
avgwt/=n;
avgtat/=n;
printf("\naverage waiting time of the above processes: %f",avgwt);
printf("\naverage turn around time of above processes: %f",avgtat);
return 0;
}
