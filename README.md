John Patrick P. Fabila
BSIT-3.8

# Week 7 Lab – Dart Fundamentals

Name: John Patrick P. Fabila

Section: BSIT-3.8

## Files

- campus_brew_receipt.dart – Campus Brew order receipt (Parts 2–8)
- print_shop.dart – Campus Print Shop bill (Part 10)

## How to run

Copy a file's code into https://dartpad.dev and click Run.

## Part 7 answers

1. Ana got the voucher because she is a student and her subtotal is more than PHP 250.

2. The delivery was not free because she did not choose pickup, and her total after the voucher was less than PHP 300.

3. We use `~/` because the points must be whole numbers, not decimals.

## Part 8 results table

| Order | Student voucher | Delivery | TOTAL | Change | Points |
|---|---|---|---|---|---|
| A – Ana | -PHP 15.50 | PHP 29.50 | PHP 310.75 | PHP 89.25 | 6 |
| A with isStudent = false | Not eligible | PHP 29.50 | PHP 326.25 | PHP 73.75 | 6 |
| B – Ben | Not eligible | FREE | PHP 295.75 | PHP 4.25 | 5 |
| C – Carla | -PHP 15.50 | FREE | PHP 321.00 | PHP 179.00 | 6 |

Carla got free delivery because her total after the voucher was PHP 321.00, which is more than PHP 300.

## Part 9 debugging table

| Bug | What DartPad said (or printed) | What was wrong | Your fixed line |
|---|---|---|---|
| 1 | Expected `;` | Missing semicolon | `String drink = 'Iced Coffee';` |
| 2 | A value of type `double` can't be assigned to `int` | Wrong data type | `double price = 65.25;` |
| 3 | The final variable `shop` can only be set once | A final variable cannot be changed | `String shop = 'Campus Brew';` |
| 4 | `Total: 25.5 * 3` | It printed the values instead of calculating them | `print('Total: ${(price * qty).toStringAsFixed(2)}');` |
| 5 | A value of type `double` can't be assigned to `int` | `/` gives a decimal value | `int boxes = cups ~/ 6;` |

## Part 10 test results

| Test | Student Name | Black Pages | Color Pages | isMember | wantsBinding | Member Discount | TOTAL | Minutes |
|---|---|---|---|---|---|---|---|---|
| 1 | Ana Reyes | 24 | 6 | true | true | -PHP 5.25 | PHP 140.00 | 3 |
| 2 | Ben Cruz | 14 | 2 | false | false | Not eligible | PHP 51.50 | 2 |
| 3 | Carla Santos | 30 | 1 | true | false | Not eligible | PHP 83.25 | 3 |

Carla did not get the discount because her subtotal is only PHP 83.25, which is less than PHP 100.

## Reflection

1. Which error message confused you the most, and how did you fix it?

The data type error confused me the most. I fixed it by checking the value and using the correct data type.

2. Where would `final` be a better choice than `var` in your receipt? Why?

`final` is better for the customer name because it should not change after it is set.

3. In a real Flutter app, where would the INPUT values come from instead of variables?

The input values would come from the user through text fields, buttons, and other input controls.
