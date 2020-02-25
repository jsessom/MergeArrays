# MergeArrays
Merge two sorted arrays and keep them sorted
#include <iostream>
using namespace std;



int main()
{
	int result[10];
	int list1[5] = { 1,8,7,9,10 };
	int list2[5] = { 6,5,4,3,2 };

	int index[10];

	for (int i = 0; i < 10; i++)
	{

		index[i] = i;
		cout << index[i] << endl;
	}
	for (int i = 0; i < result[10]; i++)
	{
		


			if (list1[index[i]] < list2[index[i]])
			{
				result[i] = list1[index[i]];

			}

			if (list1[index[i]] > list2[index[i]])
			{
				result[i] = list2[index[i]];

			}
			if (list1[index[i]] == list2[index[i]])
			{
				result[i] = list1[index[i]];

			}
			cout << result[i] << endl;
		

	}
	
}
