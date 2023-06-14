#include<iostream>
#include<conio.h>
#include<ctype.h>
#include<stdlib.h>
using namespace std;

int main(){
	
	double a,b,s,r,m,d;
	char Opc;
	
	cout<<"Selecione operacion: "<<endl;
	cout<<"a)Suma. "<<endl;
	cout<<"b)Multiplicacion. "<<endl;
	cout<<"c)Resta."<<endl;
	cout<<"d)Division."<<endl;
	cin>>Opc;
	
	switch(Opc){
		case 'a':cout<<"Ha selecionado suma: "<<endl;
		cout<<"Ingrese primer numero: "<<endl; cin>>a;
		cout<<"Ingrese segundo numero: "<<endl; cin>>b;	
		if(isdigit(a) and isdigit(b)){
		
		s=a+b;	
		cout<<"Resultado es: "<<s<<endl;
	}
	else 
	{
		cout<<"No es un numero."<<endl;
	}
		break;
		
		case 'b':cout<<"Ha selecionado Multiplicacion: "<<endl;
		cout<<"Digite primera cantidad: "<<endl;cin>>a;
		cout<<"Digite segundfa cantidad: "<<endl;cin>>b;
		m=a*b;
		cout<<"Resultado es: "<<m<<endl;
		break;
		
		case 'c': cout<<"Ha selecionado resta: "<<endl;
		cout<<"Digite primera cantidad: "<<endl;cin>>a;
		cout<<"Digite segunda cantidad: "<<endl;cin>>b;
		r=a-b;
		cout<<"Resultado es: "<<r<<endl;
		break;
		
		case 'd':cout<<"Ha selecionado Division: "<<endl;
		cout<<"Ingrese primera cantidad: "<<endl; cin>>a;
		cout<<"Ingrese segunda cantidad: "<<endl; cin>>b;
		d=a/b;
		cout<<"Resultado es: "<<d<<endl;
		break;
		
	}
}
