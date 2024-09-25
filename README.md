# C++ 2D Array - Matrices

## Aim
To study and implement C++ 2D arrays, commonly referred to as matrices.

## Software Used
Visual Studio Code.

## Theory
A 2D array in C++ is an array of arrays, meaning it's a collection of elements arranged in a grid or table with rows and columns.

### Syntax
```cpp
data_type array_name[rows][columns];
```

## Example Code
```cpp
#include <iostream>
using namespace std;

int main() {
    int i, j;
    int arr[2][3];

    cout << "Enter 6 numbers: ";
    for (i = 0; i < 2; i++) {
        for (j = 0; j < 3; j++) {
            cin >> arr[i][j];
        }
    }

    cout << "The entered matrix is:" << endl;
    for (i = 0; i < 2; i++) {
        for (j = 0; j < 3; j++) {
            cout << arr[i][j] << " ";
        }
        cout << endl;
    }

    return 0;
}
```

## Algorithm for Displaying a 2D Array

### Inputting Values into the 2D Array
1. **Start.**
2. Declare a 2D integer array `arr` with 2 rows and 3 columns.
3. Declare integer variables `i` and `j` for loop counters.
4. Display the message "Enter 6 numbers: " to prompt the user for input.
5. Use a nested for loop to input values into the 2D array `arr`:
   - **Outer loop**: Iterate `i` from 0 to 1 (for each row).
   - **Inner loop**: Iterate `j` from 0 to 2 (for each column within the current row).
   - In each iteration of the inner loop, take input from the user and store it in `arr[i][j]`.
6. **End.**

### Displaying the 2D Array
1. **Start.**
2. Use another nested for loop to print the elements of the 2D array:
   - **Outer loop**: Iterate `i` from 0 to 1 (for each row).
   - **Inner loop**: Iterate `j` from 0 to 2 (for each column within the current row).
   - In each iteration of the inner loop, print the value of `arr[i][j]` followed by a space.
   - After the inner loop completes, print a newline to move to the next row.
3. **End.**
