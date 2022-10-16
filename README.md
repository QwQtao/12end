# 12end
数组（上）


int main()
{
	int arr[10] = { 1,2,3 };//1,2,3,0,0,0,0,0,0,0
	char arr2[5] = { 'a','b' };//a,b,0,0,0
	char arr3[5] = "ab";//a,b,0 ,0,0
	return 0;
}

int main()
{
	char arr1[]
	char arr2[]
	printf("%d\n", sizeof(arr1));
	printf("%d\n", sizeof(arr2));
	printf("%d]n", strlen(arr1));
	printf("%d]n", strlen(arr2));
}

int main()
{
	char arr[] = "abcdef";
	int i = 0;
	int len = strlen(arr);
	for (i = 0; i < len; i++)
	{
		printf("%c", arr[i]);
	}
	return 0;
}

int main()
{
	int arr[] = { 1,2,3,4,5,6,7,8,9,0 };
	int sz = sizeof(arr) / sizeof(arr[0]);
	int i = 0;
	for (i = 0; i < sz; i++)
	{
		printf("%d", arr[i]);
	}
	return 0;
}

 一维数组中的存储
int main()
{
	int arr[] = { 1,2,3,4,5,6,7,8,9,0 };
	int sz = sizeof(arr) / sizeof(arr[0]);
	int i = 0;
	for (i = 0; i < sz; i++)
	{
		printf("&arr[%d]=%p\n", i, &arr[i]);
	}
	return 0;
}

//二维数组创建
int main()
{
	int main[3][4];
	char ch[5][6];
	return 0;
}

//初始化
int main()
{
	int arr[3][4] = { {1,2,3},{4,5} };
	return 0;
}

int main()
{
	int arr[][4] = { {1,2,3,4},{5,6,7,8} };
	return 0;
}

//使用下标访问
int main()
{
	int arr[3][4] = { {1,2,3},{4,5} };
	//1 2 3 0
	//4 5 0 0
	//0 0 0 0
	int i = 0;
	for (i = 0; i < 3; i++)
	{
		int j = 0;
		for (j = 0; j < 4; j++)
		{
			printf("%d ", arr[i][j]);//打印每个元素
		}
		printf("\n");//空一行
	}
	return 0;
}

int main()
{
	int arr[3][4] = { {1,2,3,},{4,5} };
	int i = 0;
	for(i=0;i<3;i++)
	{
		int j = 0;
		for (j = 0; j < 4; j++)
		printf("&arr[%d][%d]=%p\n", i, j, &arr[i][j]);
	}
	return 0;
}
