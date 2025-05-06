# bai-tu-do
project lien toan co ban
#include <iostream>
using namespace std;
void menu() {
	cout << "\n==== May tinh don gian ==\n";
	cout << "1.cong (+)\n";
	cout << "2.tru (-) \n";
	cout << "3.nhan (*)\n";
	cout << "4.chia (/)\n";
	cout << "0.thoat\n";
	cout << "chon phep toan: ";
}
int main() {
	int luachon;
	float a, b, ketqua;
	do {
		menu();
		cin >> luachon;
		if (luachon == 0) {
			cout << "tambiet";
			break;
		}
		cout << "nhap so thu nhat :";
		cin >> a;
		cout << "nhap so thu hai :";
		cin >> b;
		switch (luachon) {
		case1:
			ketqua = a + b;
			cout << "ketqua:" << a << "+" << b << "=" << ketqua << endl;
			break;
		case2 :
			ketqua = a - b;
			cout << "ketqua:" << a << "-" << b << "=" << ketqua << endl;
		case 3:
			ketqua = a * b;
			cout << "ketqua :" << a << "*" << b << "=" << ketqua << endl;
		case 4:
			if (b != 0) {
				ketqua = a / b;
				cout << "ketqua:" << a << "/" << b << "=" << ketqua << endl;

			}
			else {
				cout << "loi: khong the chia cho 0!\n";
			}
			break;
		default:
			cout << "lua chon khong hop le .\n";
		

		}

	} while (true);
	cout << endl;
	return 0;
}
