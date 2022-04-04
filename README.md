#include <iostream>
using namespace std;
int main()
{
	int size;
	cout<<"Enter the size of the array:"<<endl;
	cin>>size;
	int arr[100];
	cout<<"Enter the elements of the array: "<<endl;
	for(int i=0; i<size; i++){
		cin>>arr[i];
	}
	int temp=0;
	for(int i=0; i<size; i++)
	{
		for(int j=i+1; j<size; j++)
		{
			if(arr[i]>arr[j]){
			
			int temp=arr[i];
			arr[i]=arr[j];
			arr[j]=temp;
		}
		}
	}
	cout<<"The Ascending order of the numbers are"<<endl;
	for(int i=0; i<size; i++)
	{
	cout<<arr[i]<<" ";
	}
	return 0;
}
