#include<iostream>
#include<cstdlib>
#include<ctime>
#define tentativa 10
using namespace std;

int main(){
	
	int numero;
	int numeros1;
	int chanche[tentativa];
	int chanche2 = 1;
	
	srand(time(NULL));
	
	
	
	cout << "Digite um numero: \n";
	 cin >> numeros1;

	while(chanche2 <= tentativa){
		numero = rand() % 50;
				  
		if(numeros1 < numero){
			cout << "Mais. \n";
			cout << "Tente denovo: \n";
			cin >> numeros1;
	    
		}else if(numeros1 > numero){
			cout << "Menos. \n";
			cout << "Tente denovo: \n";
			cin >> numeros1;
		}		
		chanche2++;
	}
	
		if(numeros1 = numero){
			cout << "Parabens, voce nao ganhou, a resposta era: " << numero << "\n";	
	    }else if(chanche2 > tentativa){
			cout << "Que pena, voce nao ganhou, a resposta era: " << numero;
		}
	
system("pause");
return 0;
}
