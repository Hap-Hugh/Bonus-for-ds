#include<stdio.h>
#include<stdlib.h>

#define MAXNUM 100000

int array[MAXNUM];


int compare(const void *a, const void *b)
{
	return *(int *)a - *(int *)b;
}

int main()
{
	int n,length = 0;
	long long p;
	int i, j;
	scanf("%d%d", &n, &p);
	
	if (n != 0)
	{
		for (i = 0; i < n; i++)
		{
			scanf("%d", &array[i]);
		}
		qsort(array, n, sizeof (int), compare);
	} else {
		printf("0");
		return 0;
	}
	
	for(i = 0; i < n - 1; i++)
	{
		int thisnum = array[i];
		for(j = i + length +1; j < n; j++) {
			long long thatnum = array[j];
			long long bound = p*thisnum;
			if (bound < thatnum)
			{
				break;
			}
			else 
			{
				if(j - i > length)
					length = j - i;
			}
			
			
		}
	}
	printf("%d", length +1);
	return 0;
}
