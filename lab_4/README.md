## 1.	If the ages of Ali, Saleem and Noreen are input by the user, write a program to determine the youngest of the three (use IF statement)
```cpp
#include <iostream>

int main() {
	std::cout << "Enter Age of Ali, Saleem and Noreen: ";
	int ali{}, saleem{}, noreen{};
	std::cin >> ali >> saleem >> noreen;

	if (ali <= saleem) {
		if (ali <= noreen)
			std::cout << "Ali is Youngest!" << '\n';
		
		if (noreen < ali)
			std::cout << "Noreen is the Youngest!" << '\n';
	}

	if (saleem <= ali) {
		if (saleem <= noreen)
			std::cout << "Saleem is the Youngest!" << '\n';
		
		if (noreen < saleem)
			std::cout << "Noreen is the Youngest!" << '\n';
	}
	
	return 0;
}
```

## 2.	If the ages of Ali, Saleem and Noreen are input by the user, write a program to determine the oldest of the three (use IF…ELSE statement)
```cpp
#include <iostream>

int main() {
	std::cout << "Enter Age of Ali, Saleem and Noreen: ";
	int ali{}, saleem{}, noreen{};
	std::cin >> ali >> saleem >> noreen;

	if (ali >= saleem) {
		if (ali >= noreen)
			std::cout << "Ali is the Eldest!" << '\n';
		else
			std::cout << "Noreen is the Eldest!" << '\n';
	} else {
		if (saleem >= noreen)
			std::cout << "Saleem is the Eldest!" << '\n';
		else
			std::cout << "Noreen is the Eldest!" << '\n';
	}
	return 0;
}
```

## 3.	Write a program return absolute value of an input integer without using any built-in function.
```cpp
#include <iostream>

int main() {
	std::cout << "Enter an Integer: ";
	int n{};
	std::cin >> n;

	if (n < 0)
		n = -n;

	std::cout << "\n|" << n << "| = " << n << '\n';

	return 0;
}
```

## 4.	Write a program to check whether the uppercase or lowercase alphabet is a vowel or not using if- else statement.
```cpp
#include <iostream>

int main() {
	std::cout << "Enter a character: ";
	char C{};
	std::cin >> C;

	if (C == 'A' || C == 'a' ||
	    C == 'E' || C == 'e' ||
	    C == 'I' || C == 'i' || 
	    C == 'O' || C == 'o' ||
	    C == 'U' || C == 'u')
		std::cout << C << " is a Vowel.\n";	
	else
		std::cout << C << " is a Consonant.\n";

	return 0;
}
```
