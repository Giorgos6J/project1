# Java Console Menu Program (Scanner Tasks)

A simple Java console application that:
1) asks for your first and second name,
2) greets you,
3) repeatedly asks for a “key pass” (any integer; `0` exits),
4) lets you choose a **task number** (10–80) to run different mini-calculations.

---

## Features / Tasks

After you enter the key pass (anything except `0`), the program asks:

**“Give task number:”**  
Choose one of the following:

### Task 10 — Basic Arithmetic (2 numbers)
**Input:** `a1 a2` (two integers)  
**Output:** Sum, Difference, Modulo, Product

> Note: if `a2 = 0`, modulo (`a1 % a2`) will crash with division-by-zero.

---

### Task 20 — Triangle Type + Area/Perimeter
**Inputs:**
- height `h`
- side `a`
- side `b`
- side `c`

**Output:**
- Triangle type: Equilateral / Isosceles / Scalene
- Area = `(h * a) / 2` (integer math)
- Perimeter = `a + b + c`

> Note: Area uses **integer division**, so decimals are truncated.

---

### Task 30 — Rectangle or Square + Area/Perimeter
**Inputs:** `s1`, `s2` (two side lengths)  
**Output:**
- “Square” if `s1 == s2`, else “Rectangle”
- Area = `s1 * s2`
- Perimeter = `2 * (s1 + s2)`

---

### Task 40 — Circle Measurements
**Input:** `radius` (integer)  
**Output:**
- Diameter = `2 * radius`
- Area = `π * r²`
- Circumference = `2πr`

---

### Task 50 — Powers + Optional Square Root
**Inputs:** `s1`, `s2` (two integers)  
**Does:**
- Computes `s1^s2` and `s2^s1` (calculated but **not printed** in the current code)
- Computes `diff = s1 - s2`
- If `diff > 0`, prints `sqrt(diff)`

---

### Task 60 — Multiplication Table (1 to 10)
**Input:** `number`  
**Output:** `number * 1` through `number * 10`

---

### Task 70 — Last Digit (only if number > 100)
**Input:** `number`  
**Output:** last digit (`number % 10`) if `number > 100`

---

### Task 80 — Factors of a Number
**Input:** `number`  
**Output:** all integers that divide `number` (from `1` to `number`)

---

## How to Run

1. Make sure you have Java installed.
2. Put the code inside a class with a `main` method and a `Scanner` like:
   - `Scanner scanner = new Scanner(System.in);`
3. Compile and run:

```bash
javac Main.java
java Main
