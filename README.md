#include <iostream>
#include <fstream>
#include <vector>
#include <string>
#include <cstdlib>
using namespace std;

class program
{
	
	public:
		
		vector<string> program1;
		string napis;
		
		ifstream plik1;
    ofstream plik2;
		
		void wprowadzp1();
};

gra::gra(){
    plik1.open("c:\\1.txt");
    plik2.open("c:\\2.txt");
};

void gra::wprowadzPlik(){
	
	 int i=0;
	
	 if(plik1.good())  
      while(!plik1.eof()&i<3){
      getline(plik1, napis);
			program1.push_back(napis);i++;				
        }
};

class g1
public:
{
	string tryb;				
	
	public:
		void wprowadzx();
		void wypiszz();
};

void g1::wprowadzx(){
	wprowadzp1();
	plik1>>tryb;
};

void g1::wypiszz(){
	plik2<<"{\"nazwa"<<"\":\""<<program1[0]<<"\",\"rok\":\""<<program1[1]<<"\,\"producent\":\""
	<<program1[2]<<"\",\"tryb"<<"\":\""<<tryb<<"\"}";
};

    plik1.close();
    plik2.close();
}

int main(int argc, char** argv) {
	game1 X;
	X.wprowadzx();
	X.wypiszz();
	return 0;
}
