## 1. Practice these technique to show your efficiency in
### a)
```cpp
#include <iostream>

int main() {
    int i{ 123 };
    float f{ 1.23f };
    double d{ 1.23456f };
    char c{ 'a' };
    bool b{ true };

    std::cout << "Integer i = " << i << std::endl;
    std::cout << "Float f = " << f << std::endl;
    std::cout << "Double d = " << d << std::endl;
    std::cout << "Character c = " << c << std::endl;
    std::cout << "Boolean b = " << b << std::endl;

    return 0;
}
```

### b) Arithmetic operations
```cpp
#include <iostream>

int main() {
    std::cout << "Enter first number: ";
    double a{};
    std::cin >> a;

    std::cout << "Enter second number: ";
    double b{};
    std::cin >> b;
    
    std::cout << std::endl;
    
    std::cout << a << " + " << b << " = " << a + b << std::endl;
    std::cout << a << " - " << b << " = " << a - b << std::endl;
    std::cout << a << " * " << b << " = " << a * b << std::endl;
    std::cout << a << " / " << b << " = " << a / b << std::endl;
    
    return 0;
}
```

### c) Modulus operator
```cpp
 #include <iostream>

int main() {
    std::cout << "Enter the Dividend: ";
    int dividend{};
    std::cin >> dividend;

    std::cout << "Enter the Divisor: ";
    int divisor{};
    std::cin >> divisor;

    int quotient{ dividend / divisor };
    int remainder{ dividend % divisor };

    std::cout << std::endl;
    std::cout << dividend << " / " << divisor << std::endl;
    std::cout << "Quotient: " << quotient << std::endl;
    std::cout << "Remainder: " << remainder << std::endl;
    
    return 0;
}
```

## 2. Develop code in C++ that may convert decimal number into its equivalent binary number?
```cpp
#include <iostream>

int main() {
    std::cout << "Enter an integer: ";
    int input{};
    std::cin >> input;

    int n{ input },
        bit{},
        binary{},
        multiple{ 1 };

    while (n != 0) {
        bit = n % 2;
        binary += bit * multiple;
        n /= 2;
        multiple *= 10;
    }

    std::cout << std::endl;
    std::cout << input << " in Binary: " << binary << std::endl;

    return 0;
}
```

## 3. Write a program that may take a digit as input such as “7591” and displays that output as:
1  
9  
5  
7  
```cpp
#include <iostream>

int main() {
    std::cout << "Enter an integer: ";
    int input;
    std::cin >> input;

    std::cout << std::endl;
    
    std::cout << input % 10 << std::endl;
    std::cout << input / 10 % 10 << std::endl;
    std::cout << input / 100 % 10 << std::endl;
    std::cout << input / 1000 % 10 << std::endl;

    return 0;
}
```
