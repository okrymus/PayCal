// This program calculate gross incomes to the monitor.
// a nicely formatted table project
// The programmer: Panupong Leenawarat
// last modified 30 september 2015

#include <iostream>
#include <iomanip>
using namespace std;

int main()
{
	int time1, time2, time3, time4, time5;
	double rate1, rate2, rate3, rate4, rate5;
	double timeSum, avrPayRate, totalPay;

	cout << "\t   The program craetes a nicely formatted table\n";
	cout << "\t\t\tsample solution by\n";
	cout << "\t\t\t  Lee. Panupong\n";

	cout << "Hours worked Employee #1 [Only hours will credited]: ";
	cin >> time1; cin.ignore(80, '\n');
	cout << "Hourly pay rate for Employee #1 [not necessarily whole dollars]: ";
	cin >> rate1; cin.ignore(80, '\n');

	cout << "Hours worked Employee #1 [Only hours will credited]:";
	cin >> time2; cin.ignore(80, '\n');
	cout << "Hourly pay rate for Employee #1 [not necessarily whole dollars]: ";
	cin >> rate2; cin.ignore(80, '\n');

	cout << "Hours worked Employee #1 [Only hours will credited]:";
	cin >> time3; cin.ignore(80, '\n');
	cout << "Hourly pay rate for Employee #1 [not necessarily whole dollars]: ";
	cin >> rate3; cin.ignore(80, '\n');

	cout << "Hours worked Employee #1 [Only hours will credited]:";
	cin >> time4; cin.ignore(80, '\n');
	cout << "Hourly pay rate for Employee #1 [not necessarily whole dollars]: ";
	cin >> rate4; cin.ignore(80, '\n');

	cout << "Hours worked Employee #1 [Only hours will credited]:";
	cin >> time5; cin.ignore(80, '\n');
	cout << "Hourly pay rate for Employee #1 [not necessarily whole dollars]: ";
	cin >> rate5; cin.ignore(80, '\n');

	//Calculate the tatal hours
	timeSum = time1 + time2 + time3 + time4 + time5;
	//Calculate the average pay rates
	avrPayRate = (rate1 + rate2 + rate3 + rate4 + rate5) / 5;
	//Calculate the total pay
	totalPay = (time1*rate1) + (time2*rate2) + (time3*rate3) + (time4*rate4) + (time5*rate5);

	// Display 
	cout << setprecision(6);
	cout << "\n\tEmplyee#" << setw(15) << "Hours" << setw(15) << "Pay Rate" << setw(15) << "Total Pay" << endl;
	cout << "\t=========================================================" << endl;
	cout << setw(13) << "1" << setw(17) << time1 << setw(10) << "$" << setw(7) << rate1 << setw(7) << "$" << setw(6) << time1*rate1 << endl;
	cout << setw(13) << "2" << setw(17) << time2 << setw(10) << "$" << setw(7) << rate2 << setw(7) << "$" << setw(6) << time2*rate2 << endl;
	cout << setw(13) << "3" << setw(17) << time3 << setw(10) << "$" << setw(7) << rate3 << setw(7) << "$" << setw(6) << time3*rate3 << endl;
	cout << setw(13) << "4" << setw(17) << time4 << setw(10) << "$" << setw(7) << rate4 << setw(7) << "$" << setw(6) << time4*rate4 << endl;
	cout << setw(13) << "5" << setw(17) << time5 << setw(10) << "$" << setw(7) << rate5 << setw(7) << "$" << setw(6) << time5*rate5 << endl;
	cout << "      " << "TOTAL/AVERAGE" << setw(11) << timeSum << setw(10) << "$" << setw(7) << avrPayRate << setw(7) << "$" << setw(6) << totalPay << endl << endl;

	cout << "Please hit ENTER to terminate the program" << endl;

	system("pause");
	return 0;
}