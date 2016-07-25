#include<iostream>
using namespace std;
char nom_l2[30],nom_lb[30],nom_u[30];
bool rep=true;
int fec_a, valido=0,p=0;
struct biblioteca
{
	char nom_a[20],ape_a[20],nom_l[40],asig[30];
	int grado,tomo,fec_e,fec_p,pres=0;
}libro[1000];

void lle(struct matriz[])
{
	for(int i=0;i<1;i++)
	{
		cout<<"nombre del libro: ";
		cin>>libro[1].nom_l;
		cout<<"nombre del autor: ";
		cin>>libro[i].nom_a;
		cout<<"apellido del autor: ";
		cin>>libro[i].ape_a;
		cout<<"asignatura: ";
		cin>>libro[i].asig;
		cout<<"grado: ";
		cin>>libro[i].grado;
		cout<<"fecha de edición: ";
		cin>>libro[i].fec_e;
		cout<<"fecha de publicación";
		cin>>libro[i].fec_p;
		cout<<"tomo";
		cin>>libro[i].tomo;
	}
	cout<<endl;
	
}

struct prestamista()
{
char nom_p[20],ape_p[20],calle[20],ciudad[20],sector[20],libro_p[2][30];
	int edad,num_c.fec_v[2]={0};
}presta[1000];

void prestamo_libro()
{
	do{
		cout<<"nombre del libro";
		cin>>nom_l2;
		for(int i=0;i<1000;i++)
		{
			if(nom_12==libro[i].nom_l)
			{	
				rep=false;
				if(libro[i].pres!=0)
				{
					cout<<"no se puede prestar, el libro ya esta ocupado"<<endl;
					rep=true;
				}
				else if
				{
					libro[i].pres=1;
					prestar_libro();
				}
			}
		}
		if(rep==true)
			cout<<<"el libro ya esta prestado o no se encuentra en la lista"<<endl;
	}while(rep==true);
					
}
void borrar_libro()
{
	do{
		cout<<"nombre del libro a borrar";
		cin>>nom_lb;
		
		for(int i=0;i<1000;i++)
		{
			if(nom_lb==libro[i].nom_l)
				{
					libro[i]={0};
					cout<<"libro borrado"
					rep=false;		
				}
		}
		if(rep==true)
		cout<<"el libro no se encuentra en la lista";
	}while(rep==true);
}

void prestar_libro()
{
	rep=true;
	cout<<"nombre del usuario: ";
	cin>>nom_u;
	for(int i=0;i<1000;i++)
	{
		if(nom_u==presta[i].nom_p)
		{		
			rep=false;
			cout<<"fecha actual: ";
			cin>>fec_a;
			valido=fec_a-presta[i].fec_v[0];
			if(valido<=0)
			{
				cout<<"usted tiene un libro que entregar"<<endl;
				cout<<"el nombre del libro es: "<<presta[i].libro_p[0];
				if(presta[i].fec_v[1]==0)
				{
					cout<<"se puede prestar el libro";
					cout<<"escriba la fecha en que el usuario debe entregar el libro";
					cin>>presta[i].fec_v[1];
					cout<<"nombre del libro: ";
					cin>>presta[i].libro_p[1];
				}
				else 
					cout<<"no se puede prestar el libro ya tine dos libros prestados.";
			}
		}
	}
	if(rep==true)
	{
		p++;
		cout<<"nombre del usuario: ";
		cin>>presta[p].nom_p;
		cout<<"apellido del usuario: ";
		cin>>presta[p].ape_p;
		cout<<"edad del usuario: ";
		cin>>presta[p].edad;
		cout<<"dirección del usuario: ";
		cout<<"ciudad: "
		cin>>presta[p].ciudad;
		cout<<"sector: "
		cin>>presta[p].sector;
		cout<<"calle: "
		cin>>presta[p].calle;
		cout<<"numero de casa: "
		cin>>presta[p].num_c;
		cout<<"nombre del libro a prestar: ";
		cin>>presta[p].libro_p[0];
		cout<<"fecha de entrega: "
		cin>>presta[p].fec_v[0];
	}
}

void devolver_libro()
{
	
}
