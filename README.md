# Seconds to Day & Hour & Minutes & Seconds
#include <iostream>
#include <Cmath>
using namespace std;

void MAX_Num()
{

    int Total_Seconds = 0;

    cout << "Ente Seconds : " << endl;
    cin >> Total_Seconds;

    const int Seconds_to_Days = 24 * 60 * 60;
    const int Seconds_to_Hour = 60 * 60;
    const int Seconds_to_Minutes = 60;

    int Switch1 = floor(Total_Seconds / Seconds_to_Days);// 193535 / 84600 = 2 Days (Floor Function clear the number)
    int Remainder = Total_Seconds % Seconds_to_Days;// 193535 mod 84600 = 24.335
    int Switch2 = floor(Remainder / Seconds_to_Hour);// 24335 / 3600 = 6.75 with floor function return to smallest value 5 .
    Remainder = Remainder % Seconds_to_Hour; // 24335 mod 3600 = 2735
    int Switch3 = floor(Remainder / Seconds_to_Minutes); // 2735 / 60 = 45 
    Remainder = Remainder % Seconds_to_Minutes;// 2735 mod 60 = 35
    int Switch4 = Remainder;








    cout << "Days : " << Switch1 << " |Hours : " << Switch2 << " |Minutes : " << Switch3 << " |Seconds : " << Switch4 << endl;

    
}



int main()
{
    
    MAX_Num();
    

    return 0;
}




