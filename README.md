# first
my first repository

#include<iostream>
#include<windows.h>
#include<iomanip>
#include<string>

using namespace std;

int main()
{
	int number;
	cout<<"输入一个数字"<<endl;
	cin>>number;  
	cout<<"你输入的是:"<<number<<"\n"; 

	//cin输入空格的办法:使用getline函数(包含于string中)
	cin.ignore();    //问题在于此，如果不加入这行的话，后面getline读取时会读到上面cin的回车，导致无法输入
	string str;
	getline(cin,str);
	cout<<str<<endl;
	


	return 0;
}
