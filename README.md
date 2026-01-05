#include <iostream>
#include <iomanip>
using namespace std;

double footToMeter(double foot) {
    return 0.305 * foot;
}

double meterToFoot(double meter) {
    return meter / 0.305;
}

int main()
{
    cout << "Feet\tMeters\t|\tMeters\tFeet\n";
    for (double i = 1, m = 20; i <= 10; i++, m += 5) {
        cout << fixed << setprecision(1) << i << "\t";
        cout << setprecision(3) << footToMeter(i) << "\t|\t";
        cout << fixed << setprecision(1) << m << "\t";
        cout << setprecision(3) << meterToFoot(m) << "\n";
    }
    return 0;
}
