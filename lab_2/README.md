## 1. You should modify the program so that it produces output similar to the following.
### a)
```cpp
#include <iostream>

int main() {
    std::cout << "  *\n";
    std::cout << " * *\n";
    std::cout << "*   *\n";
    std::cout << "*   *\n";
    std::cout << "*   *\n";
    std::cout << " * *\n";
    std::cout << "  *\n";

    return 0;
}
```

### b)
```cpp
#include <iostream>

int main() {
    std::cout << "+++++++++\n";
    std::cout << "+       +\n";
    std::cout << "+       +\n";
    std::cout << "+       +\n";
    std::cout << "+       +\n";
    std::cout << "+       +\n";
    std::cout << "+++++++++\n";

    return 0;
}
```

### c)
```cpp
#include <iostream>

int main() {
    std::cout << "========\n";
    std::cout << "|      |\n";
    std::cout << "|      |\n";
    std::cout << "|      |\n";
    std::cout << "========\n";
    
    return 0;
}
```

## 2) Design C++ program output using your own imagination and innovation
```cpp
#include <iomanip>
#include <iostream>

int main() {
    std::cout << std::setw(55) << "__________________________________________" << '\n';
    std::cout << std::setw(14) << "/\\" << std::setw(42) << "\\" << '\n';
    std::cout << std::setw(12) << "/" << std::setw(3) << "\\" << std::setw(42) << "\\" << '\n';
    std::cout << std::setw(11) << "/" << std::setw(5) << "\\" << std::setw(28) << "________" << std::setw(14) << "\\" << '\n';
    std::cout << std::setw(10) << "/" << std::setw(7) << "\\" << std::setw(20) << "\\" << std::setw(4) << "\\" << std::setw(4) << "\\" << std::setw(14) << "\\" << '\n';
    std::cout << std::setw(9) << "/" << std::setw(9) << "\\" << std::setw(28) << "\\===\\===\\" << std::setw(14) << "\\" << '\n';
    std::cout << std::setw(8) << "/" << std::setw(11) << "\\" << std::setw(28) << "\\___\\___\\" << std::setw(14) << "\\" << '\n';
    std::cout << std::setw(7) << "/" << std::setw(13) << "\\" << std::setw(42) << "\\" << '\n';
    std::cout << std::setw(21) << "/______________\\" << std::setw(42) << "\\" << '\n';
    std::cout << std::setw(6) << "/:" << std::setw(16) << ":\\" << "_________________________________________\\" << '\n';
    std::cout << std::setw(6) << ":" << std::setw(15) << ":" << std::setw(43) << ":" << '\n';
    std::cout << std::setw(6) << ":" << std::setw(15) << ":" << std::setw(43) << ":" << '\n';
    std::cout << std::setw(6) << ":" << std::setw(15) << ":" << std::setw(43) << ":" << '\n';
    std::cout << std::setw(6) << ":" << std::setw(9) << "____" << std::setw(6) << ":" << std::setw(25) << "___" << std::setw(18) << ":" << '\n';
    std::cout << std::setw(6) << ":" << std::setw(5) << ":" << std::setw(5) << ":" << std::setw(5) << ":" << std::setw(26) << ":_:_:" << std::setw(17) << ":" << '\n';
    std::cout << std::setw(6) << ":" << std::setw(5) << ":" << std::setw(5) << ":" << std::setw(5) << ":" << std::setw(26) << ":_:_:" << std::setw(17) << ":" << '\n';
    std::cout << std::setw(6) << ":" << std::setw(5) << ":" << std::setw(5) << ":" << std::setw(5) << ":" << std::setw(43) << ":" << '\n';
    std::cout << std::setw(6) << ":" << std::setw(5) << ":" << std::setw(5) << "+:" << std::setw(5) << ":" << std::setw(43) << ":" << '\n';
    std::cout << std::setw(6) << ":" << std::setw(5) << ":" << std::setw(5) << ":" << std::setw(5) << ":" << std::setw(43) << ":" << '\n';
    std::cout << std::setw(6) << ":" << "____:____:____:__________________________________________:";
    return 0;
}
```
