---

# Basic Calculator in C

This project implements a basic calculator in C. It includes functions for addition, subtraction, multiplication, and division.

## Project Structure

```
c-calculator
├── README.md
├── calculator.c
└── calculator.h
```

### calculator.h

The `calculator.h` file contains the function prototypes for the basic calculator operations:

```c
#ifndef CALCULATOR_H
#define CALCULATOR_H

// Function prototypes for basic calculator operations

// Adds two numbers
float add(float a, float b);

// Subtracts the second number from the first
float subtract(float a, float b);

// Multiplies two numbers
float multiply(float a, float b);

// Divides the first number by the second
float divide(float a, float b);

#endif
```

### calculator.c

The `calculator.c` file contains the definitions of the functions declared in `calculator.h`:

```c
#include "calculator.h"

// Function definitions

// Adds two numbers
float add(float a, float b) {
    return a + b;
}

// Subtracts the second number from the first
float subtract(float a, float b) {
    return a - b;
}

// Multiplies two numbers
float multiply(float a, float b) {
    return a * b;
}

// Divides the first number by the second
float divide(float a, float b) {
    if (b != 0) {
        return a / b;
    } else {
        // Handle division by zero error
        return 0; // Alternatively, you can use error handling mechanisms
    }
}
```

---
