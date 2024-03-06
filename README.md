#include <stdio.h>
#include <conio.h>
#include <math.h>;//chua hang so pi la M_PI

void main()
{
	float pi, t, n, eps, dau;
	clrscr();
	printf("Nhap sai so eps=");
	scanf("%f", &eps);
#include <stdio.h>
#include <conio.h>

void main()
{
	int n, i, j, s, ts;
	clrscr();
	printf("Nhap n=");
	scanf("%d", &n);
	printf("Cac so hoan hao khong vuot qua %d la :", n);

	for (ts = 0, i = 2; i <= n; i++)
	{
		s = 1;
		for (j = 2; j <= i / 2; j++)
			if (i % j == 0) s += j;
		if (s == i)
		{
			ts++;
			printf("\n %d = 1", i);
			for (j = 2; j <= i / 2; j++)
				if (i % j == 0) printf(" + %d", j);
		}
	}

	if (ts) printf("\nCo tat ca %d so hoan hao", ts);
	else printf("\nKhong co so hoan hao nao");
	getch();
}
	pi = 0;
	t = 4;
	n = dau = 1;

	do
	{
		pi += dau * t;
		n = n + 2;
		dau = -dau;
		t = 4 / n;
	} while (t >= eps);
	printf("\nSo PI tinh duoc voi sai so %12.10f, PI=%12.10f\n", eps, pi);
	printf("\nSo PI cua Turbo C++, PI=%12.10f\n", M_PI);
	getch();
}# -#include <stdio.h>
#include <conio.h>

void main()
{
	int n, i, j, s, ts;
	clrscr();
	printf("Nhap n=");
	scanf("%d", &n);
	printf("Cac so hoan hao khong vuot qua %d la :", n);

	for (ts = 0, i = 2; i <= n; i++)
	{
		s = 1;
		for (j = 2; j <= i / 2; j++)
			if (i % j == 0) s += j;
		if (s == i)
		{
			ts++;
			printf("\n %d = 1", i);
			for (j = 2; j <= i / 2; j++)
				if (i % j == 0) printf(" + %d", j);
		}
	}

	if (ts) printf("\nCo tat ca %d so hoan hao", ts);
	else printf("\nKhong co so hoan hao nao");
	getch();
}
