## Write a program that will compute the area of a circle. The user must enter the radius of the circle. Use the following formula for area A = 3.14 R^2.
```cpp
#include <iostream>

int main() {
    std::cout << "Enter the Radius of Circle:" << std::endl;
    std::cout << "> ";

    double r{};
    std::cin >> r;

    double area {3.14 * r * r};
    std::cout << "Area: " << area << std::endl;
    
    return 0;
}
```

## Write a program that will solve for the power dissipation of a resistor when the voltage across the resistor and the current in the resistor are known as I=5A and R=16ohm. The relationship for power dissipation is: P=I^2 * R, where P = Power dissipated, I = resistor current, V= resistor voltage.
```cpp
#include <iostream>

int main() {
    int I {5}; // Current I = 5A
    int R {16}; // Resistance R = 16 ohm
    int P {I * I * R}; // Power P = I^2 * R

    std::cout << "Current I: " << I << 'A' << std::endl;
    std::cout << "Resistance R: " << R << " ohm" << std::endl;

    std::cout << std::endl;
    
    std::cout << "Power P = I^2 * R = " << P << 'W' << std::endl;
    return 0;
}
```

## Which one should be preferred, a Compiler or an Interpreter? Explain why?
A compiler produces more optimal and executable code than an interpreter, which can be more efficient and faster. But changes require you to recompile your program.  
An interpreter allows you to easily see your changes in code without having to recompile but it is slower compared to compiler.
