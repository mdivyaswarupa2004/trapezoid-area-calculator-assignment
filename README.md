# Trapezoid Area Calculator

A Java application that calculates the area of a trapezoid using the formula: **Area = ((a + b) / 2) × h**

## Project Overview

This project implements a trapezoid area calculator following a structured Git workflow with multiple feature branches that depend on each other.

## Author

**M.Divyaswarupa**

EMAIL:divyaswarupa@everest.engineering

🔗 Repository: [trapezoid-calculator](git@github.com:mdivyaswarupa2004/trapezoid-area-calculator-assignment.git)

## Formula

**Trapezoid Area = ((a + b) / 2) × h**

Where:
- `a` = length of first parallel side
- `b` = length of second parallel side  
- `h` = height of the trapezoid

## Features

- **Addition Operation**: Adds two values (a + b)
- **Division by Two**: Divides any value by 2
- **Multiplication**: Multiplies division result by height
- **Complete Calculation**: Full trapezoid area calculation

## Project Structure
trapezoid-calculator/
├ TrapezoidCalculator.java    # Main calculator implementation
├ README.md                   # Main project documentation

├ feature/addition/
   |--    README.md              # Addition feature documentation
├ feature/divisionByTwo/
   |-- README.md              # Division by 2 feature documentation
└ feature/multiplication/
    |-- README.md              # Multiplication feature documentation

## Requirements

- **Java Development Kit (JDK)**: Version 8 or higher
- **Git**: For version control operations
- **Command Line Interface**: Terminal or Command Prompt

## Installation & Setup

Download JDK:

Oracle JDK: <https://www.oracle.com/java/technologies/downloads/>

OpenJDK (Free):<https://openjdk.org/install/>

1. **Clone the repository**:

   ```bash
   git clone [git@github.com:mdivyaswarupa2004/trapezoid-area-calculator-assignment.git]
   cd trapezoid-calculator
   ```

2. **Verify Java installation**:

   ```bash
   java -version
   javac -version
   ```

## How to Run

1. **Compile the Java file**:

   ```bash
   javac TrapezoidCalculator.java
   ```

2. **Run the application**:

   ```bash
   java TrapezoidCalculator
   ```

3. **Expected Output**:

   ```bash
   Trapezoid Area Calculator
   Given: a=4, b=6, h=5
   Step 1 - Addition (a+b): 10
   Step 2 - Division by 2: 5
   Step 3 - Multiplication by h: 25
   Final Area: 25
   ```

## Git Workflow & Branch Strategy

This project follows Challenge-2 requirements with complex branching and rebasing:

### Branch Structure

```bash
main
├ feature/addition
├ feature/divisionByTwo
│   └ feature/multiplication (created on top of divisionByTwo)
```


## Assignment Steps Implementation

### Challenge-2 Step-by-Step

**Step 1**: Initial commit with main file in master branch

- Created `TrapezoidCalculator.java` with basic structure

**Step 2**: Create `feature/divisionByTwo` branch

- Implements dividing given value by 2
- Example: Input=6 -> Output=3

**Step 3**: Create `feature/addition` branch  

- Implements adding a and b values
- Example: a=2, b=3 -> Output=5

**Step 4**: Create `feature/multiplication` on top of `feature/divisionByTwo`

- Implements multiplication by height h
- Example: divisionValue=2, h=3 -> Output=6

**Step 5**: Merge `feature/addition` with master branch

**Step 6**: Rebase `feature/divisionByTwo` with master

- Get addition logic in divisionByTwo branch
- Calculate (a+b)/2 using both addition and division logic

**Step 7**: Merge `feature/divisionByTwo` into master

**Step 8**:Get all code from master in `feature/multiplication`

- Perform final calculation: ((a+b)/2) × h

## Branch Status

- **feature/addition**: Complete and merged
- **feature/divisionByTwo**: Complete, rebased, and merged
- **feature/multiplication**: Complete with final integration
- **main**: Contains all merged features

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For any questions or suggestions:

- **Email**:divyaswarupa@everest.engineering
- **GitHub**:[git@github.com:mdivyaswarupa2004/trapezoid-area-calculator-assignment.git]
