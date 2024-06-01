# Mean-Median-of-array
To find the mean and median of a user input array
//Mean and median of an array
#include<iostream>
#include<algorithm>
using namespace std;

int main(){
	int n;
	cout<<"Enter the size of array: ";
	cin>>n;
	int arr[n],sum=0;
	for(int i=0;i<n;i++){
		cin>>arr[i];
		sum+=arr[i];
	}
	cout<<"Mean is: "<<sum/n<<endl;
	sort(arr,arr+n);
	if(n%2==0){
		cout<<"Median is: "<<(arr[(n/2)-1]+arr[n/2])/2;
	}
	else{
		cout<<"Median is: "<<arr[n/2];
	}
	
}
