#include <iostream>
using namespace std;
int sum(int x, int y){
return x+y;
}
int razn(int x, int y){
    return x-y;
}
int umn(int x, int y){
    return x*y;
}
int razd(int x,int y){
    return x/y;
}
int ost(int x,int y){
    return x%y;
}
int LU(int x,int y){
    return x&y;
}
int LS(int x,int y){
    return x|y;
}
int XOR(int x,int y){
    return x^y;
}
int SDL(int x,int y){
    return x << y;
}
int SDR(int x,int y){
    return x>>y;
}
int main()
{ 
int i;
int x;
int y;
char op1,op;
cin >>x;
cin >>op;
if (op=='>') 
{
cin>>op1;
}
else if(op=='<') 
{
cin>>op1;
}
cin>>y;


if( op == '+' ) {
cout << sum(x, y) << endl;
}
else if( op == '-' ) 
{
cout << razn(x, y) << endl;
}
else if( op == '*' ) 
{
cout << umn(x, y)<< endl;
}
else if( op == '/' ) 
{
if (y==0) 
{
cout<<"error"<<endl;
}
else
cout << razd(x, y) << endl;
}

else if( op == '%' ) 
{
cout << ost(x, y) << endl;
}
else if( op == '&' ) 
{
cout << LU(x, y)<< endl;
}
else if( op == '|' ) 
{
cout << LS(x, y) << endl;
}
else if( op == '^' ) 
{
cout << XOR(x, y) << endl;
}
else if( op == '/' ) 
{
cout << razd(x, y) << endl;
}
else if (op=='<',op1=='<') 
{
cout << SDL(x, y) << endl;
}
else if (op=='>',op1=='>') 
{
cout << SDR(x, y) << endl;
}
else 
{
cout << "wrong operator" << endl;
}
cin.get();
return 0;

}
