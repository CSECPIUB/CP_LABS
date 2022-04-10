## Design and develop a marks certificate for 5 subjects, showing obtained marks and total marks for each subject. The marks certificate should also display total obtained percentage/ SGPA in the semester?
```cpp
#include <iomanip>
#include <stdlib.h> // for system(args);
#include <iostream>

int main() {
    system("cls"); // clear screen

    int LA{}, CS{}, CAG{}, CP{}, PST{};
    std::cout << "Enter Marks for Liner Algebra (Max 50): ";
    std::cin >> LA;

    double LA_PERCENTAGE{ LA / 50.0 * 100.0 };
    double LA_GPA{ (LA_PERCENTAGE >= 85.0 && LA_PERCENTAGE <= 100.0) ? 4.0 :
                    (LA_PERCENTAGE >= 72.5 && LA_PERCENTAGE <= 85.0) ? 3.0 :
                    (LA_PERCENTAGE >= 62.5 && LA_PERCENTAGE <= 72.5) ? 2.0 :
                    (LA_PERCENTAGE >= 52.5 && LA_PERCENTAGE <= 62.5) ? 1.0 : 0.0 };
    double LA_GRADE{ LA_GPA * 2 };

    std::cout << "Enter Marks for Communication Skills (Max 50): ";
    std::cin >> CS;

    double CS_PERCENTAGE{ CS / 50.0 * 100.0 };
    double CS_GPA{ (CS_PERCENTAGE >= 85.0 && CS_PERCENTAGE <= 100.0) ? 4.0 :
                    (CS_PERCENTAGE >= 72.5 && CS_PERCENTAGE <= 85.0) ? 3.0 :
                    (CS_PERCENTAGE >= 62.5 && CS_PERCENTAGE <= 72.5) ? 2.0 :
                    (CS_PERCENTAGE >= 52.5 && CS_PERCENTAGE <= 62.5) ? 1.0 : 0.0 };
    double CS_GRADE{ CS_GPA * 2 };

    std::cout << "Enter Marks for Calculus (Max 100): ";
    std::cin >> CAG;

    double CAG_PERCENTAGE{ CAG / 100.0 * 100.0 };
    double CAG_GPA{ (CAG_PERCENTAGE >= 85.0 && CAG_PERCENTAGE <= 100.0) ? 4.0 :
                    (CAG_PERCENTAGE >= 72.5 && CAG_PERCENTAGE <= 85.0) ? 3.0 :
                    (CAG_PERCENTAGE >= 62.5 && CAG_PERCENTAGE <= 72.5) ? 2.0 :
                    (CAG_PERCENTAGE >= 52.5 && CAG_PERCENTAGE <= 62.5) ? 1.0 : 0.0 };
    double CAG_GRADE{ CAG_GPA * 3 };

    std::cout << "Enter Marks for Computer Programming (Max 100): ";
    std::cin >> CP;

    double CP_PERCENTAGE{ CP / 100.0 * 100.0 };
    double CP_GPA{ (CP_PERCENTAGE >= 85.0 && CP_PERCENTAGE <= 100.0) ? 4.0 :
                    (CP_PERCENTAGE >= 72.5 && CP_PERCENTAGE <= 85.0) ? 3.0 :
                    (CP_PERCENTAGE >= 62.5 && CP_PERCENTAGE <= 72.5) ? 2.0 :
                    (CP_PERCENTAGE >= 52.5 && CP_PERCENTAGE <= 62.5) ? 1.0 : 0.0 };
    double CP_GRADE{ CP_GPA * 3 };

    std::cout << "Enter Marks for Pakistan Studies (Max 50): ";
    std::cin >> PST;
    
    double PST_PERCENTAGE{ PST / 50.0 * 100.0 };
    double PST_GPA{ (PST_PERCENTAGE >= 85.0 && PST_PERCENTAGE <= 100.0) ? 4.0 :
                    (PST_PERCENTAGE >= 72.5 && PST_PERCENTAGE <= 85.0) ? 3.0 :
                    (PST_PERCENTAGE >= 62.5 && PST_PERCENTAGE <= 72.5) ? 2.0 :
                    (PST_PERCENTAGE >= 52.5 && PST_PERCENTAGE <= 62.5) ? 1.0 : 0.0 };
    double PST_GRADE{ PST_GPA * 2 };

    int obtained{ LA + CS + CAG + CP + PST };
    double total{ 350.0 };
    double totalCredit{ 12.0 };
    double obtainedGrade{ LA_GRADE + CS_GRADE + CAG_GRADE + CP_GRADE + PST_GRADE };
    double percentage{ obtained / total * 100.0 };
    double sgpa{ obtainedGrade / totalCredit };

    std::cout << std::endl << std::endl;
    std::cout << std::setw(20) << "Subject"                 << std::setw(15) << "Obtained" << std::setw(10) << "Total" << std::setw(15) << "Percentage"                       << std::setw(10) << "Grade"        << std::setw(10) << "GPA"   << std::setw(10) << "SGPA" << std::endl;
    std::cout << std::endl;
    std::cout << std::setw(20) << "Linier Algebra"          << std::setw(15) << LA         << std::setw(10) << 50      << std::setw(15) << LA_PERCENTAGE                      << std::setw(10) << LA_GRADE       << std::setw(10) << LA_GPA                             << std::endl;
    std::cout << std::setw(20) << "Communication Skills"    << std::setw(15) << CS         << std::setw(10) << 50      << std::setw(15) << CS_PERCENTAGE                      << std::setw(10) << CS_GRADE       << std::setw(10) << LA_GPA                             << std::endl;
    std::cout << std::setw(20) << "Calculus"                << std::setw(15) << CAG        << std::setw(10) << 100     << std::setw(15) << CAG_PERCENTAGE                     << std::setw(10) << CAG_GRADE      << std::setw(10) << LA_GPA                             << std::endl;  
    std::cout << std::setw(20) << "Computer Programming"    << std::setw(15) << CP         << std::setw(10) << 100     << std::setw(15) << CP_PERCENTAGE                      << std::setw(10) << CP_GRADE       << std::setw(10) << LA_GPA                             << std::endl;
    std::cout << std::setw(20) << "Pakistan Studies"        << std::setw(15) << PST        << std::setw(10) << 50      << std::setw(15) << PST_PERCENTAGE                     << std::setw(10) << PST_GRADE      << std::setw(10) << LA_GPA                             << std::endl;
    std::cout << std::endl;
    std::cout << std::setw(20) << "Total"                   << std::setw(15) << obtained   << std::setw(10) << total   << std::setw(15) << std::setprecision(2) << percentage << std::setw(20) << obtainedGrade  << std::setw(10)                             << sgpa   << std::endl;
    std::cout << std::endl;
    
    system("pause");
    return 0;
}
```

##  Write a program to make an arithmetic calculator using if-else if statement
```cpp
#include <iostream>

int main() {
    std::cout << "Enter 1st Number: ";
    double num1{};
    std::cin >> num1;

    std::cout << "Enter 2nd Number: ";
    double num2{};
    std::cin >> num2;

    std::cout << "Enter the Operation (+, -, /, *): ";
    char op{};
    std::cin >> op;

    double result{};

    std::cout << std::endl;

    if (op == '+')
        result = num1 + num2;
    else if (op == '-')
        result = num1 - num2;
    else if (op == '*')
        result == num1 * num2;
    else if (op == '/')
        result = num1 / num2;
    else
        std::cout << "Invalid Input!" << std::endl;

    std::cout << num1 << " " << op << " " << num2 << " = " << result << std::endl;
    
    return 0;
}
```

##On November 01, 2021 Government decided to increase/decrease petrol prices. There are two options under consideration for petrol price increase...
```cpp
#include <iostream>

int main() {
    std::cout << "Enter Increase in Price (2 or 3 Rupees): ";
    int increase{};
    std::cin >> increase;

    (increase == 2) ? std::cout << "Sugar Price is 105 Rupees!\n" :
    (increase == 3) ? std::cout << "Sugar Price is 108 Rupees!\n" :
    std::cout << "Invalid Increase!\n";

    return 0;
}
```
