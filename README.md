# C_Class_190730_2
입력한 두 수와 그 사이 값들의 합


#include <stdio.h>

//입력한 두 수와 그 사이의 모든 값들의 합
void main()
{
	int n1, n2, s = 0, i;
	scanf_s("%d", &n1);
	scanf_s("%d", &n2);
	printf("\n");
	if (n1 > n2) //n1이 클 때
		for (i = n2; i < n1; i++)
		{
			printf("%d  \n", i);
		}
	else //n1이 크지 않을 때
		for (i = n1; i <= n2; i++)
		{
			s += i;
			printf("%d  \n", i);
		}
	printf("=	%d \n",s);
}


/*
#include <stdio.h>

//입력한 두 수와 그 사이의 모든 값들의 합
void main()
{
	int n1, n2, s = 0, i;
	scanf_s("%d", &n1);
	scanf_s("%d", &n2);
	printf("\n");
	if (n1 > n2)
		for (i = n1; i >= n2; i--) //첫 번째 값이 두 번째 입력값보다 같거나 크면 줄어든다.
		{
			s += i; //i를 더한 값들을 s에 넣는다.
			printf("첫 번째 입력 값 : %d\n", i);
		}
	else
		for (i = n1; i <= n2; i++)
		{
			s += i;
			printf("두 번째 입력 값 : %d\n", i);
		}
	printf("= %d	\n", s);
}
*/



/*
//가장 짧고 효율적인(?) 코딩
#include <stdio.h>
void main()
{
	int n1, n2, s = 0, i, p; //p는 피난값
	printf("시작값과 끝값을 차례로 입력하세요. >> ");
	scanf_s("%d %d", &n1, &n2);
	printf("\n");
	if (n1 >n2);
		p = n1, n1 = n2, n2 = p;
	for (i = n1; 1 <= n2; i++)
		{
			s += i;
			printf("%d ", i);
			if (i == n2) printf("=");
			else printf("+ ");
		}
	printf(" %d \n", s);
}
*/
