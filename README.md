# Currency_converter
#include<iostream>
#include<conio.h>  
using namespace std;
// Function to convert Pakistani currency.
double convertpkrinusd(double amount)
{
return amount * 0.012;
}
double convertpkrinPound(double amount)
{
return amount * 0.0092;
}
double convertpkrinEuro(double amount)
{
return amount * 0.010;
}
double convertpkrinYen(double amount)
{
return amount * 1.43;
}
double convertpkrinLira(double amount)
{
return amount * 0.14;
}

// Functions to convert USD.
double convertusdinPkr(double amount)
{
return 84.80 * amount;
}
double convertusdinEuro(double amount)
{
return 0.91 * amount;
}
double convertusdinPound(double amount)
{
return 0.75 * amount;
}
double convertusdinYen(double amount)
{
return 112.09 * amount;
}
double convertusdinLira(double amount)
{
return amount * 8.97;
}

// Functions to convert GBP
double convertgbpinusd(double amount)
{
return amount * 1.18;
}
double convertgbpinPkr(double amount)
{
return amount / 249.15;
}
double convertgbpinEuro(double amount)
{
return amount * 1.08;
}
double convertgbpinYen(double amount)
{
return amount / 154.95;
}
double convertgbpinLira(double amount)
{
return amount / 11.40;
}

// Functions to convert euro.
double converteurinPkr(double amount)
{
return amount * 109.76;
}
double converteurinPound(double amount)
{
return amount * 0.93;
}
double converteurinYen(double amount)
{
return amount * 129.60;
}
double converteurinLira(double amount)
{
return amount * 10.22;
}
double converteurinusd(double amount)
{
return amount * 1.10;
}

// Function to convert Lira.
double converttryinPkr(double amount)
{
return amount * 81.22;
}
double converttryinPound(double amount)
{
return amount * 0.025;
}
double converttryinYen(double amount)
{
return amount * 4.68;
}
double converttryinusd(double amount)
{
return amount * 0.011;
}
double converttryineuro(double amount)
{
return amount * 0.098;
}

// Function to convert JPY.
double convertjpyinLira(double amount)
{
return amount * 0.21;
}
double convertjpyinPkr(double amount)
{
return amount * 1.92;
}
double convertjpyinPound(double amount)
{
return amount * 0.0077;
}
double convertjpyinusd(double amount)
{
return amount * 0.0089;
}
double convertjpyineuro(double amount)
{
return amount * 0.0081;
}

int main()
{
// Code used to change the color of the output
system("color 2f");

int n;
string choice;
do
{
string currency;
cout << "You can convert 6 currencies which are listed below:\n"
    << "Select the currency which is to be converted (type in CAPITAL).\n"
    << "If dollars then type (USD) \nIf UK pounds then type (GBP) \nIf Euro then type (EUR)\nIf Turkish Lira then type (TRY)\nIf Japanese Yen then type (JPY)\nIf Pakistani Rupee then type (PKR)\n";
cout << "Type the type of currency in CAPITAL ALPHABET'S : ";
cin >> currency;
system("color 3F");
cout << "Enter the amount of " << currency << " : ";
cin >> n;

system("color 03");

if(currency == "USD") // CHANGE THE CURRENCIES IN DOLLAR
{
cout << "_____________________" << endl;
cout << "| $ | " << n << " | Dollar in Pakistan Rupees will be | " << convertusdinPkr(n) << " Rupees " << endl;
cout << "| $ | " << n << " | Dollar in UK pounds will be       | " << convertusdinPound(n) << " POUNDS " << endl;
cout << "| $ | " << n << " | Dollar in Euro will be            | " << convertusdinEuro(n) << " EUROS   " << endl;
cout << "| $ | " << n << " | Dollar in Turkish Lira will be    | " << convertusdinLira(n) << " TRY     " << endl;
cout << "| $ | " << n << " | Dollar in Japanese Yen will be    | " << convertusdinYen(n) << " YEN      " << endl;
cout << "_____________________" << endl;
}
else if(currency == "GBP")  // CHANGE THE CURRENCIES AMOUNT IN POUNDS
{
cout << "__________________________" << endl;
cout << "| � | " << n << " | Pound sterling in Pakistan Rupees will be | : " << convertgbpinPkr(n) << " Rupees " << endl;
cout << "| � | " << n << " | Pound sterling in US Dollars will be      |: " << convertgbpinusd(n) << " POUNDS " << endl;
cout << "| � | " << n << " | Pound sterling in Euro will be            |: " << convertgbpinEuro(n) << " EUROS " << endl;
cout << "| � | " << n << " | Pound sterling in Turkish Lira will be:   |" << convertgbpinLira(n) << " TRY " << endl;
cout << "| � | " << n << " | Pound sterling in Japanese Yen will be:   |" << convertgbpinYen(n) << " YEN " << endl;
cout << "__________________________" << endl;
}

else if(currency == "EUR")       //CHANGE THE CURREINCES IN EURO
{
cout << "_______________________" << endl;
cout << "| � | " << n << " | Euro in Pakistan Rupees will be         | " << converteurinPkr(n) << " Rupees " << endl;
cout << "| � | " << n << " | Euro in US Dollars will be              | " << converteurinusd(n) << " DOLLARS " << endl;
cout << "| � | " << n << " | Euro in Pound sterling will be          | " << converteurinPound(n) << " POUNDS " << endl;
cout << "| � | " << n << " | Euro in Turkish Lira will be            | " << converteurinLira(n) << " TRY " << endl;
cout << "| � | " << n << " | Euro in Japanese Yen will be            | " << converteurinYen(n) << " YEN " << endl;
cout << "_______________________" << endl;
}
else if(currency == "TRY")
{
cout << "________________________" << endl;
cout << "| " << n << " | Turkish Lira in Pakistan Rupees will be :      |" << converttryinPkr(n) << " Rupees " << endl;
cout << "| " << n << " | Turkish Lira in US Dollars will be :           |" << converttryinusd(n) << " DOLLARS " << endl;
cout << "| " << n << " | Turkish Lira in Pound sterling will be :       |" << converttryinPound(n) << " POUNDS " << endl;
cout << "| " << n << " | Turkish Lira in Euro will be :                 |" << converttryineuro(n) << " EUROS " << endl;
cout << "| " << n << " | Turkish Lira in Japanese Yen will be :         |" << converttryinYen(n) << " YEN " << endl;
cout << "________________________" << endl;
}

else if(currency == "JPY")
{
cout<<"______________________"<<endl;
cout << "| � | " << n << " | Japanese Yen in Pakistan Rupees will be  | " << convertjpyinPkr(n) << " Rupees " << endl;
cout << "| � | " << n << " | Japanese Yen in US Dollars will be       | " << convertjpyinusd(n) << " DOLLARS " << endl;
cout << "| � | " << n << " | Japanese Yen in Pound sterling will be   | " << convertjpyinPound(n) << " POUNDS " << endl;
cout << "| � | " << n << " | Japanese Yen in Turkish Lira will be     | " << convertjpyinLira(n) << " TRY " << endl;
cout << "| � | " << n << " | Japanese Yen in Euro will be             | " << convertjpyineuro(n) << " EUROS " << endl;
cout<<"______________________"<<endl;

}

else if(currency == "PKR")
{
cout << "______________________" << endl;
cout << "| RS " << n << " | Pakistan Rupees in Euro will be :             |" << convertpkrinEuro(n) << " EUROS " << endl;
cout << "| RS " << n << " | Pakistan Rupees in US Dollars will be :       |" << convertpkrinusd(n) << " DOLLARS " << endl;
cout << "| RS " << n << " | Pakistan Rupees in Pound sterling will be :   |" << convertpkrinPound(n) << " POUNDS " << endl;
cout << "| RS " << n << " | Pakistan Rupees in Turkish Lira will be :     |" << convertpkrinLira(n) << " TRY " << endl;
cout << "| RS " << n << " | Pakistan Rupees in Japanese Yen will be :     |" << convertpkrinYen(n) << " YEN " << endl;
cout << "______________________" << endl;
}
else
{
cout << "\nEnter a registered currency. Any other entry other than the above-mentioned entries will not be accepted.\n";
}

cout << "\nIf you want to try again then type (YES), if not then type (NO)\nChoose : ";
cin >> choice;
system("color 8f");
}
while(choice == "YES");
getche();
return 0;
}

