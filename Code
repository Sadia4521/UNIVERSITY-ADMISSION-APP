#include<iostream>
#include<string.h>
using namespace std;
void form()
{
	int day, month, year;
	char dash;
	string gender, matric, intermediate, password;
	char name[15], fn[15], arr[50], sch[25], col[25], e[50], f[25], n[15], m[15];
cout << "\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^UNIVERSITY APPLICATION FORM^^^^^^^^^^^^^^^^^^^^^^^^^^^^ ";
	cout << "\n         ";
	cout << " \n---------------------------      ";
	cout << "\nPERSONAL INFORMATION:";
	cout << " \n---------------------------   ";
	cout << "\nEnter your Email:";
	cin.ignore();
	cin.get(e, 50);
	cout << "\nEnter your password:";
	cin >> password;
	cout << "\nEnter your Full Name:   ";
	cin.ignore();
	cin.get(name, 15);
	cout << "\nEnter your father Full Name:   ";
	cin.ignore();
	cin.get(fn, 25);
	cout << "\nEnter your Date of Birth:   ";//Enter your date of birth (dd-mm-yyyy)
	cin >> day >> dash >> month >> dash >> year;
	cout << "\nEnter your CNIC number :";
	cin.ignore();
	cin.get(n, 15);
	cout << "\nEnter your father CNIC number :";
	cin.ignore();
	cin.get(m, 15);
	cout << "\nEnter your Gender:  ";
	cin >> gender;
	cout << "\nEnter your Address:  ";
	cin.ignore();
	cin.get(arr, 50);
	cout << "\n------------------------      ";
	cout << "\nACADEMIC BACKGROUND:";
	cout << "\n------------------------     ";
	cout << "\nEnter the field you want to apply in : ";
	cin.ignore();
	cin.get(f, 25);
	cout << "\nEnter Your School Name :";
	cin.ignore();
	cin.get(sch, 25);
	cout << "\nEnter your group name of matric :";//e.g : biology;computer;humanity
	cin >> matric;
	cout << "\nEnter Your college Name :";
	cin.ignore();
	cin.get(col, 25);
	cout << "\nEnter your group name of intermediate :";//e.g : fsc;ics;FA
	cin >> intermediate;
	cout << "\n     ";
	cout << "\nThank you for filling the form";
	cout << "\n---------------------------------------------------------------------";
}
void merit(string name)
{
if (name == "bahria" || name == "foundation" || name == "gift" || name == "allama iqbal" || name == "national defence university")
		cout << "Your merit must be 55 percent else you cannot apply for this university";
	else if (name == "nust" || name == "fast" || name == "air" || name == "comsats")
		cout << "Your merit must be 70 percent else you cannot apply for this university";
	else if (name == "ripha")
		cout << "Your merit must be 40 percent else you cannot apply for this university";
}
void feevoucher(string name)
{
if (name == "bahria" || name == "foundation" || name == "gift" || name == "allama iqbal" || name == "national defence university")
	{
		cout << "\n---------------------------------------------------------------------";
		cout << "\nYour fee voucher for this university is";
		cout << "\nYour entry test fee : 1200";
		cout << "\nOther credential : 800";
		cout << "\nYour total fee : 2000";
		cout << "\n---------------------------------------------------------------------";
	}
	else if (name == "nust" || name == "fast" || name == "air" || name == "comsats")
	{
		cout << "\n---------------------------------------------------------------------";
		cout << "\nYour fee voucher for this university is";
		cout << "\nYour entry test fee : 1800";
		cout << "\nOther credential : 1200";
		cout << "\nYour total fee : 3000";
		cout << "\n---------------------------------------------------------------------";
	}
	else if (name == "ripha")
	{
		cout << "\n---------------------------------------------------------------------";
		cout << "\nYour fee voucher for this university is";
		cout << "\nYour entry test fee : 1500";
		cout << "\nOther credential : 1000";
		cout << "\nYour total fee : 2500";
		cout << "\nYour admit card for test of each university will be send to you through Email";
		cout << "\n---------------------------------------------------------------------";
	}
}
int main()
{
	char c;
	string name;
cout << "\n********************WELCOME TO THE UNIVERSITY ADMISSION APP********************";
	cout << "\nOur app deal with following 10 universities";
cout << "\n BAHRIA UNIVERSITY \n COMSATS UNIVERSITY\n FOUNDATION UNIVERSITY \n GIFT UNIVERSITY GUJRANWALA \n RIPHA INTERNATIONAL UNIVERSITY \n AIR UNIVERSITY \n FAST UNIVERSITY \n ALLAMA IQBAL UNIVERSITY\n NATIONAL DEFENCE UNIVERSITY \n NUST UNIVERSITY ";
	cout << "\nYou can apply only in these 10 universities";
	form();
	do
	{
		int matric, fsc, nts;	
		cout << "\nEnter the name of university you want to apply in" << endl;
		cin >> name;
		merit(name);
		cout << "\nEnter the number of matric:";
		cin >> matric;
		cout << "\nEnter the number of fsc:";
		cin >> fsc;
		cout << "\nEnter the number of NTS:";
		cin >> nts;
		int merit = matric * 30 / 1000 + fsc * 40 / 1000 + nts * 30 / 100;
		if (name == "nust")
		{
			int NAT;
			cout << "Enter the NAT marks";
			cin >> NAT;
			int merit = matric * 30 / 1000 + fsc * 40 / 1000 + nts * 10 / 100 + NAT * 20 / 100;
		}
		cout << "\nYour merit is " << merit << "%";
		if (merit < 40)
		{
cout << "\nSorry your merit is too low  you cannot apply in any of these universities";
			break;
		}
if (name == "bahria" || name == "foundation" || name == "gift" || name == "allama iqbal" || name == "national defence university")
		{
			if (merit < 55)
cout << "\nSorry your merit is low for this university you cannot apply in this university ";
			else
				feevoucher(name);
		}
		else if (name == "nust" || name == "fast" || name == "air" || name == "comsats")
		{
			if (merit < 70)
cout << "\nSorry your merit is low for this university you cannot apply in this university ";
			else
				feevoucher(name);
		}
		else if (name == "ripha")
		{
			if (merit < 40)
cout << "\nSorry your merit is low for this university you cannot apply in this university and you also cannot apply in any else university ";
			else
				feevoucher(name);
			break;
		}
		else
			cout << "   ";
		cout << "\nIf you don't want to apply for any else university enter n";
		cin >> c;
	} while (c != 'n');
	cout << "\nThank you for using our app. I hope you enjoyed it!";
	return 0;
}
