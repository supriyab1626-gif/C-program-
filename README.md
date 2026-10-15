# C-program-

C PROGRAMMING EXERCISES - 43 programs (Exercises 2 to 60)
Each program is separate: copy one block at a time into its own .c file.

======================================================================
PROGRAM 2  (ex02_find_average_and_sum.c)
======================================================================
// Exercise No: 2 – Find Average & Sum
#include <stdio.h>

int main()
{
    float a, b, c;
    float sum, average;

    printf("Enter three numbers (a, b, c): ");
    scanf("%f%f%f", &a, &b, &c);

    sum = a + b + c;
    average = sum / 3;

    printf("Sum = %.2f\n", sum);
    printf("Average = %.2f\n", average);

    return 0;
}


======================================================================
PROGRAM 3  (ex03_simple_interest.c)
======================================================================
// Exercise No: 3 – To Find the Simple Interest
#include <stdio.h>

int main()
{
    float principal, rate, time, simple_interest;

    printf("Enter principal amount: ");
    scanf("%f", &principal);

    printf("Enter Annual rate of interest (%%): ");
    scanf("%f", &rate);

    printf("Enter Time period (in years): ");
    scanf("%f", &time);

    simple_interest = (principal * rate * time) / 100;

    printf("Simple interest = %.2f\n", simple_interest);
    printf("Total Amount payable = %.2f\n", principal + simple_interest);

    return 0;
}


======================================================================
PROGRAM 4  (ex04_uppercase_to_lowercase.c)
======================================================================
// Exercise No: 4 – To Convert the Uppercase Letter to Lowercase Letter
#include <stdio.h>

int main()
{
    char ch, lowerch;

    printf("Enter an uppercase letter: ");
    scanf("%c", &ch);

    lowerch = ch + 32;

    printf("Lowercase letter: %c\n", lowerch);

    return 0;
}


======================================================================
PROGRAM 5  (ex05_area_perimeter_of_circle.c)
======================================================================
// Exercise No: 5 – Find the Area and Perimeter of a Circle
#include <stdio.h>

int main()
{
    float radius, area, perimeter;
    float pi = 3.14159;

    printf("Enter the radius of the circle: ");
    scanf("%f", &radius);

    area = pi * radius * radius;
    perimeter = 2 * pi * radius;

    printf("Area of the circle = %.2f\n", area);
    printf("Perimeter of the circle = %.2f\n", perimeter);

    return 0;
}


======================================================================
PROGRAM 7  (ex07_area_of_rectangle.c)
======================================================================
// Exercise No: 7 – To Find the Area of a Rectangle
#include <stdio.h>

int main()
{
    float length, breadth, area;

    printf("Enter the length of the rectangle (l): ");
    scanf("%f", &length);

    printf("Enter the breadth of the rectangle (b): ");
    scanf("%f", &breadth);

    area = length * breadth;

    printf("Area of the rectangle = %.2f\n", area);

    return 0;
}


======================================================================
PROGRAM 8  (ex08_multiply_two_numbers.c)
======================================================================
// Exercise No: 8 – To Find Multiply Two Numbers
#include <stdio.h>

int main()
{
    float num1, num2, product;

    printf("Enter first number: ");
    scanf("%f", &num1);

    printf("Enter second number: ");
    scanf("%f", &num2);

    product = num1 * num2;

    printf("product = %.2f\n", product);

    return 0;
}


======================================================================
PROGRAM 11  (ex11_string_input.c)
======================================================================
// Exercise No: 11 – Program to Take String Input in C Programming
#include <stdio.h>
#define MAX_LENGTH 100

int main()
{
    char input[MAX_LENGTH];

    printf("Enter a string: ");
    scanf("%s", input);

    printf("You entered: %s\n", input);

    return 0;
}


======================================================================
PROGRAM 12  (ex12_work_with_datatypes.c)
======================================================================
// Exercise No: 12 – Write a Program to Work with Datatypes
#include <stdio.h>

int main()
{
    char c = 'a';
    int num = 10;
    float f = 1.20;
    float f1 = 1;
    double d = 3.2325467;

    printf("%c\n", c);
    printf("%d\n", num);
    printf("%f\n", f);
    printf("%f\n", f1);
    printf("%lf\n", d);

    return 0;
}


======================================================================
PROGRAM 13  (ex13_feet_to_inches.c)
======================================================================
// Exercise No: 13 – Write a Program to Convert Feet to Inches
#include <stdio.h>

int main()
{
    float feet, inches;

    printf("Enter measurement in feet: ");
    scanf("%f", &feet);

    inches = feet * 12;

    printf("%.2f feet is equal to %.2f inches\n", feet, inches);

    return 0;
}


======================================================================
PROGRAM 14  (ex14_display_residential_address.c)
======================================================================
// Exercise No: 14 – Write a Program to Display Your Residential Address
#include <stdio.h>

int main()
{
    printf("--- Residential Address ---\n");
    printf("Latha\n");
    printf("123 Elm Street, Apt 4B\n");
    printf("Springfield, IL 62701\n");
    printf("United States\n");

    return 0;
}


======================================================================
PROGRAM 15  (ex15_akshat_bank_balance.c)
======================================================================
// Exercise No: 15 – Akshat Bank Balance Calculation
#include <stdio.h>

int main()
{
    int old_balance = 45000;
    int lottery_amount = 157800;
    int current_balance;

    current_balance = old_balance + lottery_amount;

    printf("Current Bank Balance = RS %d\n", current_balance);

    return 0;
}


======================================================================
PROGRAM 16  (ex16_prateek_home_library.c)
======================================================================
// Exercise No: 16 – Prateek's Home Library Calculation
#include <stdio.h>

int main()
{
    int books_per_shelf = 483;
    int number_of_shelves = 32;
    int total_books;

    total_books = books_per_shelf * number_of_shelves;

    printf("Total number of books in Prateek's library = %d\n", total_books);

    return 0;
}


======================================================================
PROGRAM 18  (ex18_arithmetic_operations.c)
======================================================================
// Exercise No: 18 – C Program to Calculate Sum, Difference, Product, Division, and Remainder of Two Numbers
#include <stdio.h>

int main()
{
    int a, b;

    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);

    printf("Sum = %d\n", a + b);
    printf("Difference = %d\n", a - b);
    printf("Product = %d\n", a * b);
    printf("Division = %d\n", a / b);
    printf("Remainder = %d\n", a % b);

    return 0;
}


======================================================================
PROGRAM 29  (ex29_electricity_bill.c)
======================================================================
// Exercise No: 29 – Domestic Electricity Bill Calculation
#include <stdio.h>

int main()
{
    int units;
    float bill = 0;

    printf("Enter Total Units Consumed: ");
    scanf("%d", &units);

    if (units <= 100)
    {
        bill = 0;
    }
    else if (units <= 200)
    {
        bill = units * 2.5;
    }
    else if (units <= 500)
    {
        bill = units * 4.0;
    }
    else
    {
        bill = units * 6.0;
    }

    printf("Total Bill Amount = Rs. %.2f\n", bill);

    return 0;
}


======================================================================
PROGRAM 30  (ex30_employee_salary_structure.c)
======================================================================
// Exercise No: 30 – Employee Salary Structure Calculation
#include <stdio.h>

int main()
{
    int id;
    char name[50];
    float basic, hra, da, ma;
    float pf, pt, gross, deductions, net;

    printf("Enter Employee ID: ");
    scanf("%d", &id);

    printf("Enter Employee Name: ");
    scanf("%s", name);

    printf("Enter Basic Pay: ");
    scanf("%f", &basic);

    hra = basic * 0.20;
    da = basic * 0.40;
    ma = 1200;

    gross = basic + hra + da + ma;

    pf = basic * 0.12;
    pt = 200;

    deductions = pf + pt;
    net = gross - deductions;

    printf("\nGross Salary = Rs.%.2f", gross);
    printf("\nTotal Deductions = Rs.%.2f", deductions);
    printf("\nNet Salary = Rs.%.2f\n", net);

    return 0;
}


======================================================================
PROGRAM 31  (ex31_electricity_bill_slab.c)
======================================================================
// Exercise No: 31 – Electricity Bill Calculation (Slab Based)
#include <stdio.h>

int main()
{
    int units;
    float bill = 0;

    printf("Enter total units consumed: ");
    scanf("%d", &units);

    if (units <= 100)
    {
        bill = 0;
    }
    else if (units <= 200)
    {
        bill = (units - 100) * 1.5;
    }
    else if (units <= 500)
    {
        bill = (100 * 1.5) + (units - 200) * 3.0;
    }
    else
    {
        bill = (100 * 1.5) + (300 * 3.0) + (units - 500) * 6.0;
    }

    printf("Total Electricity Bill = Rs. %.2f\n", bill);

    return 0;
}


======================================================================
PROGRAM 32  (ex32_ola_ride_fare.c)
======================================================================
// Exercise No: 32 – Ola Ride Fare Calculation
#include <stdio.h>

int main()
{
    int type;
    float distance, fare = 0;

    printf("Select Vehicle Type (1: Micro, 2: Mini, 3: Prime): ");
    scanf("%d", &type);

    printf("Enter Distance in km: ");
    scanf("%f", &distance);

    if (type == 1)
    {
        fare = distance * 10;
    }
    else if (type == 2)
    {
        fare = distance * 12;
    }
    else if (type == 3)
    {
        fare = distance * 15;
    }
    else
    {
        printf("Invalid vehicle type selected.\n");
        return 0;
    }

    printf("Total Ride Fare = Rs. %.2f\n", fare);

    return 0;
}


======================================================================
PROGRAM 33  (ex33_employee_gross_net_salary.c)
======================================================================
// Exercise No: 33 – Employee Gross and Net Salary Calculation
#include <stdio.h>

int main()
{
    int id;
    char name[50];
    float basic, hra, da, ma;
    float pf, pt, gross, deductions, net;

    printf("Enter Employee ID: ");
    scanf("%d", &id);

    printf("Enter Employee Name: ");
    scanf("%s", name);

    printf("Enter Basic Pay: ");
    scanf("%f", &basic);

    hra = basic * 0.20;
    da = basic * 0.40;
    ma = 1200;

    pf = basic * 0.12;
    pt = 200;

    gross = basic + hra + da + ma;
    deductions = pf + pt;
    net = gross - deductions;

    printf("\nEmployee ID = %d", id);
    printf("\nEmployee Name = %s", name);
    printf("\nGross Salary = Rs.%.2f", gross);
    printf("\nTotal Deductions = Rs.%.2f", deductions);
    printf("\nNet Salary = Rs.%.2f\n", net);

    return 0;
}


======================================================================
PROGRAM 34  (ex34_sum_of_array.c)
======================================================================
// Exercise No: 34 – Sum of Array Elements
#include <stdio.h>

int main()
{
    int a[100], n, i, sum = 0;

    printf("Enter Number of elements: ");
    scanf("%d", &n);

    printf("Enter the Elements:\n");
    for (i = 0; i < n; i++)
    {
        scanf("%d", &a[i]);
        sum = sum + a[i];
    }

    printf("Sum = %d\n", sum);

    return 0;
}


======================================================================
PROGRAM 35  (ex35_sum_of_matrix.c)
======================================================================
// Exercise No: 35 – Sum of Matrix Elements
#include <stdio.h>

int main()
{
    int a[10][10], r, c, i, j, sum = 0;

    printf("Enter rows and columns: ");
    scanf("%d%d", &r, &c);

    printf("Enter Matrix elements:\n");
    for (i = 0; i < r; i++)
    {
        for (j = 0; j < c; j++)
        {
            scanf("%d", &a[i][j]);
            sum = sum + a[i][j];
        }
    }

    printf("Sum of Matrix elements = %d\n", sum);

    return 0;
}


======================================================================
PROGRAM 36  (ex36_odd_or_even.c)
======================================================================
// Exercise No: 36 – Find Odd or Even
#include <stdio.h>

int main()
{
    int n;

    printf("Enter a Number: ");
    scanf("%d", &n);

    if (n % 2 == 0)
    {
        printf("%d is Even\n", n);
    }
    else
    {
        printf("%d is Odd\n", n);
    }

    return 0;
}


======================================================================
PROGRAM 37  (ex37_transpose_of_matrix.c)
======================================================================
// Exercise No: 37 – Transpose of Matrix
#include <stdio.h>

int main()
{
    int a[10][10], t[10][10];
    int r, c, i, j;

    printf("Enter rows and columns: ");
    scanf("%d%d", &r, &c);

    printf("Enter matrix Elements:\n");
    for (i = 0; i < r; i++)
    {
        for (j = 0; j < c; j++)
        {
            scanf("%d", &a[i][j]);
        }
    }

    for (i = 0; i < r; i++)
    {
        for (j = 0; j < c; j++)
        {
            t[j][i] = a[i][j];
        }
    }

    printf("Transpose matrix:\n");
    for (i = 0; i < c; i++)
    {
        for (j = 0; j < r; j++)
        {
            printf("%d ", t[i][j]);
        }
        printf("\n");
    }

    return 0;
}


======================================================================
PROGRAM 38  (ex38_print_first_n_natural_numbers.c)
======================================================================
// Ex. No. 38: Write a program to print first N natural numbers using while loop
/*
ALGORITHM:
1. Start
2. Read n
3. Set i = 1
4. While i <= n, print i
5. Increment i
6. Stop
*/

#include <stdio.h>

int main() {
    int n, i = 1;
    printf("Enter N: ");
    scanf("%d", &n);

    while (i <= n) {
        printf("%d ", i);
        i++;
    }

    return 0;
}


======================================================================
PROGRAM 41  (ex41_print_n_natural_numbers_reverse.c)
======================================================================
// Ex. No. 41: Write a program to print the N natural numbers in reverse order
//             (Ex. 9, 8, 7, ... 2, 1) using a for loop. Input an initial and final value.
/*
ALGORITHM:
1. Start
2. Read initial value
3. Read final value
4. Start i from final
5. Print i
6. Decrease i
7. Repeat until i reaches initial
8. Stop
*/

#include <stdio.h>

int main() {
    int initial, final, i;

    printf("Enter initial value: ");
    scanf("%d", &initial);

    printf("Enter final value: ");
    scanf("%d", &final);

    for (i = final; i >= initial; i--) {
        printf("%d ", i);
    }

    return 0;
}


======================================================================
PROGRAM 42  (ex42_sum_of_digits.c)
======================================================================
// Ex. No. 42: Write a program to find the sum of digits using while loop
/*
ALGORITHM:
1. Start
2. Read n
3. Get last digit using % 10
4. Add digit to sum
5. Remove last digit / 10
6. Display sum
7. Stop
*/

#include <stdio.h>

int main() {
    int n, digit, sum = 0;

    printf("Enter number: ");
    scanf("%d", &n);

    while (n > 0) {
        digit = n % 10;
        sum = sum + digit;
        n = n / 10;
    }

    printf("Sum of digit = %d", sum);

    return 0;
}


======================================================================
PROGRAM 43  (ex43_check_palindrome_number.c)
======================================================================
// Ex. No. 43: Write a program to check whether a given number is a palindrome or not
/*
ALGORITHM:
1. Start
2. Read n
3. Store original number
4. Find reverse using while loop
5. Compare original and reverse
6. If equal, palindrome
7. Otherwise, not palindrome
8. Stop
*/

#include <stdio.h>

int main() {
    int n, original, reverse = 0, digit;

    printf("Enter number: ");
    scanf("%d", &n);

    original = n;

    while (n > 0) {
        digit = n % 10;
        reverse = reverse * 10 + digit;
        n = n / 10;
    }

    if (original == reverse) {
        printf("Palindrome number");
    } else {
        printf("Not a palindrome number");
    }

    return 0;
}


======================================================================
PROGRAM 44  (ex44_check_adam_number.c)
======================================================================
// Ex. No. 44: Write a program to check whether a given number is an ADAM number or not
/*
ALGORITHM:
1. Start
2. Read n
3. Find square of n
4. Reverse n
5. Find square of reversed number
6. Reverse square of n
7. Compare both values
8. If equal, ADAM number
9. Otherwise, not ADAM
10. Stop
*/

#include <stdio.h>

int reverse(int n) {
    int r = 0;
    while (n > 0) {
        r = r * 10 + n % 10;
        n = n / 10;
    }
    return r;
}

int main() {
    int n, sq, rev, revsq;

    printf("Enter number: ");
    scanf("%d", &n);

    sq = n * n;
    rev = reverse(n);
    revsq = rev * rev;

    if (reverse(sq) == revsq) {
        printf("ADAM number");
    } else {
        printf("Not an ADAM number");
    }

    return 0;
}


======================================================================
PROGRAM 45  (ex45_check_armstrong_number.c)
======================================================================
// Ex. No. 45: Write a program to check whether a given number is an Armstrong number or not
/*
ALGORITHM:
1. Start
2. Read the number
3. Store n in temp
4. Set sum = 0
5. Using do while
6. Repeat until n = 0
7. If sum == temp, print Armstrong number
8. Otherwise, print not a Armstrong number
9. Stop
*/

#include <stdio.h>

int main() {
    int n, temp, digit, sum = 0;

    printf("Enter number: ");
    scanf("%d", &n);

    temp = n;

    do {
        digit = n % 10;
        sum = sum + digit * digit * digit;
        n = n / 10;
    } while (n != 0);

    if (sum == temp) {
        printf("Armstrong number");
    } else {
        printf("Not an Armstrong number");
    }

    return 0;
}


======================================================================
PROGRAM 46  (ex46_check_perfect_number.c)
======================================================================
// Ex. No. 46: Write a program to check whether a given number is a perfect number or not
/*
ALGORITHM:
1. Start
2. Read n
3. Find factor from 1 to n-1
4. Add all factor
5. Compare sum with n
6. If equal, Perfect number
7. Otherwise, Not perfect
8. Stop
*/

#include <stdio.h>

int main() {
    int n, i, sum = 0;

    printf("Enter number: ");
    scanf("%d", &n);

    for (i = 1; i < n; i++) {
        if (n % i == 0) {
            sum = sum + i;
        }
    }

    if (sum == n) {
        printf("Perfect number");
    } else {
        printf("Not perfect number");
    }

    return 0;
}


======================================================================
PROGRAM 47  (ex47_multiplication_table.c)
======================================================================
// Ex. No. 47: Write a program to print the multiplication table using for loop
/*
ALGORITHM:
1. Start
2. Read n
3. Set i = 1
4. Calculate n x i
5. Print result
6. Increment i
7. Repeat until i = 10
8. Stop
*/

#include <stdio.h>

int main() {
    int n, i;

    printf("Enter number: ");
    scanf("%d", &n);

    for (i = 1; i <= 10; i++) {
        printf("%d x %d = %d\n", n, i, n * i);
    }

    return 0;
}


======================================================================
PROGRAM 48  (ex48_reverse_of_number.c)
======================================================================
// Ex. No. 48: Write a program to print the reverse of a number using while loop
/*
ALGORITHM:
1. Start
2. Read n
3. Get last digit
4. Add digit to reverse
5. Remove last digit
6. Repeat until n = 0
7. Display reverse
8. Stop
*/

#include <stdio.h>

int main() {
    int n, reverse = 0, digit;

    printf("Enter number: ");
    scanf("%d", &n);

    while (n > 0) {
        digit = n % 10;
        reverse = reverse * 10 + digit;
        n = n / 10;
    }

    printf("Reverse = %d", reverse);

    return 0;
}


======================================================================
PROGRAM 49  (ex49_print_numbers_reverse_range.c)
======================================================================
// Ex. No. 49: Write a program to print numbers from final value down to initial value using a for loop
#include <stdio.h>

int main() {
    int initial, final, i;

    printf("Enter initial value: ");
    scanf("%d", &initial);

    printf("Enter final value: ");
    scanf("%d", &final);

    for (i = final; i >= initial; i--) {
        printf("%d ", i);
    }

    return 0;
}


======================================================================
PROGRAM 50  (ex50_power_of_n_numbers.c)
======================================================================
// Ex. No. 50: Write a program to calculate power of n numbers using for loop
/*
ALGORITHM:
1. Start
2. Read base and exponent
3. Set power = 1
4. Multiply power by base, exponent times
5. Display power
6. Stop
*/

#include <stdio.h>

int main() {
    int base, exponent, i;
    int power = 1;

    printf("Enter base: ");
    scanf("%d", &base);

    printf("Enter exponent: ");
    scanf("%d", &exponent);

    for (i = 1; i <= exponent; i++) {
        power = power * base;
    }

    printf("power = %d", power);

    return 0;
}


======================================================================
PROGRAM 51  (ex51_arithmetic_calculator_switch.c)
======================================================================
// Ex. No. 51: Write a program to create arithmetic calculator using switch statement
/*
ALGORITHM:
1. Start
2. Read two numbers
3. Read operator
4. Use switch
5. Perform selected operation
6. Display result
7. Stop
*/

#include <stdio.h>

int main() {
    float a, b;
    char op;

    printf("Enter two numbers: ");
    scanf("%f %f", &a, &b);

    printf("Enter operator (+ - * /): ");
    scanf(" %c", &op);  // Note: space before %c handles trailing newline characters

    switch (op) {
        case '+':
            printf("Result = %.2f\n", a + b);
            break;
        case '-':
            printf("Result = %.2f\n", a - b);
            break;
        case '*':
            printf("Result = %.2f\n", a * b);
            break;
        case '/':
            if (b != 0) {
                printf("Result = %.2f\n", a / b);
            } else {
                printf("Error: Division by zero\n");
            }
            break;
        default:
            printf("Invalid Operator\n");
    }

    return 0;
}


======================================================================
PROGRAM 52  (ex52_day_of_week_switch.c)
======================================================================
// Ex. No. 52: Write a C program to print Day of a week using switch statement
/*
ALGORITHM:
1. Start
2. Read Day number
3. Use switch
4. Display corresponding day
5. Stop
*/

#include <stdio.h>

int main() {
    int day;

    printf("Enter day number (1-7): ");
    scanf("%d", &day);

    switch (day) {
        case 1:
            printf("Monday");
            break;
        case 2:
            printf("Tuesday");
            break;
        case 3:
            printf("Wednesday");
            break;
        case 4:
            printf("Thursday");
            break;
        case 5:
            printf("Friday");
            break;
        case 6:
            printf("Saturday");
            break;
        case 7:
            printf("Sunday");
            break;
        default:
            printf("Invalid Day");
    }

    return 0;
}


======================================================================
PROGRAM 53  (ex53_days_in_month_switch.c)
======================================================================
// Ex. No. 53: Write a program to print number of days in a month using switch statement
#include <stdio.h>

int main() {
    int month;

    printf("Enter month number: ");
    scanf("%d", &month);

    switch (month) {
        case 1:
        case 3:
        case 5:
        case 7:
        case 8:
        case 10:
        case 12:
            printf("31 days");
            break;
        case 4:
        case 6:
        case 9:
        case 11:
            printf("30 days");
            break;
        case 2:
            printf("28 or 29 days");
            break;
        default:
            printf("Invalid month number");
    }

    return 0;
}


======================================================================
PROGRAM 54  (ex54_check_adam_number.c)
======================================================================
// Ex. No. 54: Check if a Number is an Adam Number
/*
ALGORITHM:
1. Read Number
2. Find reverse of the number
3. Find square of original number
4. Find square of reversed number
5. Reverse the square of reversed number
6. Compare this with square of original number
7. Display result
*/

#include <stdio.h>

int reverse(int n) {
    int r, rev = 0;
    while (n != 0) {
        r = n % 10;
        rev = rev * 10 + r;
        n = n / 10;
    }
    return rev;
}

int main() {
    int n, rev, sq1, sq2;

    printf("Enter Number: ");
    scanf("%d", &n);

    rev = reverse(n);
    sq1 = n * n;
    sq2 = rev * rev;

    if (reverse(sq2) == sq1) {
        printf("ADAM number");
    } else {
        printf("Not ADAM number");
    }

    return 0;
}


======================================================================
PROGRAM 55  (ex55_check_armstrong_number.c)
======================================================================
// Ex. No. 55: Check if a Number is an Armstrong Number
/*
ALGORITHM:
1. Read Number
2. Store original number
3. Extract each digit
4. Add cube of each digit
5. Compare sum with original number
6. Display result
*/

#include <stdio.h>

int main() {
    int n, original, digit, sum = 0;

    printf("Enter Number: ");
    scanf("%d", &n);

    original = n;

    while (n != 0) {
        digit = n % 10;
        sum = sum + digit * digit * digit;
        n = n / 10;
    }

    if (sum == original) {
        printf("Armstrong Number");
    } else {
        printf("Not an Armstrong Number");
    }

    return 0;
}


======================================================================
PROGRAM 56  (ex56_check_perfect_number.c)
======================================================================
// Ex. No. 56: Check if a Number is a Perfect Number
/*
ALGORITHM:
1. Read Number
2. Set sum = 0
3. Find factors from 1 to n/2
4. Add factors to sum
5. Compare sum with original number
6. Display result
*/

#include <stdio.h>

int main() {
    int n, i, sum = 0;

    printf("Enter Number: ");
    scanf("%d", &n);

    for (i = 1; i <= n / 2; i++) {
        if (n % i == 0) {
            sum = sum + i;
        }
    }

    if (sum == n) {
        printf("Perfect Number");
    } else {
        printf("Not a Perfect Number");
    }

    return 0;
}


======================================================================
PROGRAM 57  (ex57_multiplication_table.c)
======================================================================
// Ex. No. 57: Print Multiplication Table using for Loop
/*
ALGORITHM:
1. Read Number
2. Set i = 1
3. Multiply Number by i
4. Print result
5. Increment i
6. Repeat up to 10
*/

#include <stdio.h>

int main() {
    int n, i;

    printf("Enter Number: ");
    scanf("%d", &n);

    for (i = 1; i <= 10; i++) {
        printf("%d x %d = %d\n", i, n, i * n);
    }

    return 0;
}


======================================================================
PROGRAM 58  (ex58_swap_without_third_variable.c)
======================================================================
// Ex. No. 58: Swap Two Numbers Without Using a Third Variable
/*
ALGORITHM:
1. Start
2. Read two numbers a and b
3. Add a and b and store in a (a = a + b)
4. Subtract b from a and store in b (b = a - b)
5. Subtract b from a and store in a (a = a - b)
6. Display swapped values
7. Stop
*/

#include <stdio.h>

int main() {
    int a, b;

    printf("Enter two numbers (a and b): ");
    scanf("%d %d", &a, &b);

    a = a + b;
    b = a - b;
    a = a - b;

    printf("After swapping: a = %d, b = %d\n", a, b);

    return 0;
}


======================================================================
PROGRAM 59  (ex59_power_of_number.c)
======================================================================
// Ex. No. 59: Calculate Power of a Number using for Loop
/*
ALGORITHM:
1. Start
2. Read base and exponent
3. Set power = 1
4. Repeat exponent times
5. Multiply power by base
6. Display power
7. Stop
*/

#include <stdio.h>

int main() {
    int base, exponent, i;
    int power = 1;

    printf("Enter base: ");
    scanf("%d", &base);

    printf("Enter exponent: ");
    scanf("%d", &exponent);

    for (i = 1; i <= exponent; i++) {
        power = power * base;
    }

    printf("Power = %d\n", power);

    return 0;
}


======================================================================
PROGRAM 60  (ex60_power_of_n_numbers.c)
======================================================================
// Ex. No. 60: Calculate Power of N Numbers using for Loop
/*
ALGORITHM:
1. Start
2. Read base and exponent
3. Set power = 1
4. Multiply power by base, exponent times
5. Display power
6. Stop
*/

#include <stdio.h>

int main() {
    int base, exponent, i;
    int power = 1;

    printf("Enter base: ");
    scanf("%d", &base);

    printf("Enter exponent: ");
    scanf("%d", &exponent);

    for (i = 1; i <= exponent; i++) {
        power = power * base;
    }

    printf("Power = %d\n", power);

    return 0;
}
