#include <iostream>
#include <string>
#include <vector>
using namespace std;

// Function to calculate total spending
double calculateTotalSpending(const vector<double>& spending) {
    double total = 0;
    for (double amount : spending) {
        total += amount;
    }
    return total;
}

// Function to provide financial advice
void financialAdvice(double income, double totalSpending) {
    double savings = income - totalSpending;
    
    cout << "\n--- Financial Summary ---\n";
    cout << "Total Income: $" << income << endl;
    cout << "Total Spending: $" << totalSpending << endl;
    cout << "Savings: $" << savings << endl;

    if (savings > (0.2 * income)) {
        cout << "Great job! You are saving over 20% of your income.\n";
    } else if (savings > 0) {
        cout << "Consider reducing unnecessary expenses to increase your savings.\n";
    } else {
        cout << "You're spending more than you earn. Time to re-evaluate your budget!\n";
    }
}

// Main function
int main() {
    double income;
    int numCategories;
    vector<string> categories;
    vector<double> spending;

    // Get the user's monthly income
    cout << "Enter your monthly income: $";
    cin >> income;

    // Get the number of spending categories
    cout << "How many spending categories do you have? ";
    cin >> numCategories;

    // Input spending categories and amounts
    for (int i = 0; i < numCategories; i++) {
        string category;
        double amount;

        cout << "Enter category #" << (i + 1) << " name: ";
        cin >> category;
        categories.push_back(category);

        cout << "Enter amount spent on " << category << ": $";
        cin >> amount;
        spending.push_back(amount);
    }

    // Calculate total spending
    double totalSpending = calculateTotalSpending(spending);

    // Provide financial advice
    financialAdvice(income, totalSpending);

    return 0;
}
