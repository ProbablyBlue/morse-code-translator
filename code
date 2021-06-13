#include <iostream>
#include <fstream>
#include <string>
using namespace std;
int main()
{
	char text[44]={' ','A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z','1','2','3','4','5','6','7','8','9','0','.',',','?','!',':','"','='};
	string morse[44]={"/",".-","-...","-.-.","-..",".","..-.","--.","....","..",".---","-.-",".-..","--","-.","---",".--.","--.-",".-.","...","-","..-","...-",".--","-..-","-.--","--..",".----","..---","...--","....-",".....","-....","--...","---..","----.","-----",".-.-.-","--..--","..--..","..--.","---...",".-..-.","-...-"};	
	string textToChange="";
	string newText="";
	string savedText[100];
	char choice;
	cout<<"Select 1 to convert English text to Morse code.\nSelect 2 to convert Morse code to English text."<<endl;
	cin>>choice;
	if(choice=='1')
	{
		cout<<"Enter English text.\n";
		cin.get();
		getline(cin,textToChange);
		for(int i=0;i<textToChange.size();i++)
			for(int j=0;j<44;j++)
			{
				if(textToChange[i]==text[j])	
				{
					newText+=morse[j];
					newText+=" ";
					break;
				}
			}
		cout<<"Morse Code: ";
	}
	else if(choice=='2')
	{
		cout<<"Enter Morse code.\n";
		cin.get();
		getline(cin,textToChange);
		int k=0;
		for(int i=0;i<textToChange.size();i++)
			{
				if(textToChange[i]!=' ')
				{
					savedText[k]=savedText[k]+textToChange[i];
				}
				else
					k++;
			}
		for(int i=0;i<=k;i++)
			for(int j=0;j<44;j++)
			{
				if(savedText[i]==morse[j])
				{
					newText+=text[j];
					break;
				}
			}
	}
	cout<<newText;
	return 0;
}	
