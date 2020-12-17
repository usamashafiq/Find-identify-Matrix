#include<iostream>
#include<conio.h>
using namespace std;
void main() {
	
	int  m[4][4];
	for (int row = 0; row < 4; row++) {
		cout << "Enter a number" << endl;
		for (int col = 0; col < 4; col++) {
			cin >> m[row][col];
		}

	}int q = 0,w=0,e=0;
	for (int row = 0; row < 4; row++) {
		for (int col = 0; col < 4; col++) {
			if (m[q][col] == 1) {
				w += 1;
			}
				if (m[row][col] == 0) {
					e += 1;
				}
		
		
			q++;
		}
	} 
	if (w == 4 && e == 12) {
		cout << "Its a identity matrix ";
	}
	else {
		cout << "its not a identity matrix";
}
	_getch();
}
