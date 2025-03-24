# linear-search
#include<stdio.h>
int main()
{
	int array[]={10, 2, 4,5,7,70};

	int value;
	int pos=-1;
	printf("Enter the value: ");
	scanf("%d", &value);

	for(int i=0;i<6;i++)
	{
		if(value==array[i])
		{
			pos=i+1;//store position(1-based index)
			break;//Exit loop once value is found
		}
	}
	if(pos==-1)
	{
		printf("The value is not found ");

	}
	else
	{
		printf("The value is at %d position", pos );
	}
}
