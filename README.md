#include <iostream>
using namespace std;
int main(){
	
	int n;
	//deklarasi variabel
	cout<<"Jumlah pemilik Griya Asri : ";
	cin>>n;
	cout<<endl;
	string nama [n];
	string alamat [n];
	//array n untuk nama dan alamat, sehingga jumlah nama dan alamat akan sejumlah input yang dimasukkan
	
	
	//looping pertama untuk menentukan banyak rumah dan siapa pemiliknya
	for(int a=0; a<n; a++){
		cout<<"Masukkan nama pemilik rumah "<<a+1<<": ";
		cin>>nama [a];
		cout<<"Masukkan alamat pemilik rumah "<<a+1<<": ";
		cin>>alamat [a];
		cout<<endl;
	}
	
	string x, y;
	//variabel x dan y untuk melakukan pengecekan
	cout<<"=============================================="<<endl;
		cout<<"Masukkan pemilik rumah yang ingin di cek : ";
		cin>>x;
		cout<<"Masukkan alamat rumah yang ingin di cek : ";
		cin>>y;
		cout<<endl;
		
		//percabangan untuk pengecekan rumah
		if (x==nama[0] && y==alamat[0]){
			cout<<"rumah ditemukan!";
			}else if (x==nama[1] && y==alamat[1]){
				cout<<"rumah ditemukan!";
			}else{
				cout<<"rumah tidak ditemukan";
			}
		
			
	return 0;
}
