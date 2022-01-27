#include<iostream>
using namespace std;

int main() {
	int room = 1;

	string input;

	do {

		switch (room) {
		case 1:



			cout << " You are in room 1, you can go down" << endl;
			cin >> input;
			if (input == "down")
				room = 2;

			else
				cout << " sorry not an option" << endl;

				break;


		case 2:



			cout << " You are in room 2, you can go down" << endl;
			cin >> input;
			if (input == "down")
				room = 3;

			else if (input == " up")
				room = 1;

			else
				cout << " sorry not an option" << endl;

				break;




		case 3:



			cout << " You are in room 3, you can go to the right or the left" << endl;
			cin >> input;
			if (input == "right")
				room = 5;

			else if (input == "left")
				room = 4;

			else
				cout << " sorry not an option" << endl;

			break;




		case 4:



			cout << " You are in room 4, you can go to the right" << endl;
			cin >> input;
			if (input == "right")
				room = 3;

			else
				cout << " sorry not an option" << endl;

			break;



		case 5:



			cout << " You are in room 5, you can go to the left" << endl;
			cin >> input;
			if (input == "left")
				room = 3;

			

			else
				cout << " sorry not an option" << endl;

			break;
		}
	} while (input != "q");
}
