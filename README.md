# Feature: Multiplication Implementation

This branch implements the final multiplication step for completing the trapezoid area calculation.

## Purpose

This branch completes the trapezoid area calculation by implementing the multiplication by height (h) in the formula: **((a + b) / 2) × h**

## What This Branch Does

### Implementation Details

- **Function**: Multiplies division result by height (h)
- **Input**: Division result and height value
- **Output**: Final trapezoid area
- **Formula**: Takes (a+b)/2 and multiplies by h

### Code Implementation

```java
public static double multiplication(double divisionValue, int h) {
    return divisionValue * h;
}
```

## Test Cases

### Example from Assignment

- **Input**: divisionValue = 2, h = 3
- **Output**: 6
- **Complete Example**: ((4+6)/2) × 3 = 5 × 3 = 15

## Branch Information

- **Branch Name**: `feature/multiplication`
- **Parent Branch**: `feature/divisionByTwo` (NOT main)
- **Purpose**: Complete trapezoid area calculation
- **Challenge**: Challenge-2, Step 4 & Step 8

## Unique Branch Position

This branch has a special creation pattern:

```bash
main
|- feature/addition
|- feature/divisionByTwo
  |- feature/multiplication (this branch - created ON TOP of divisionByTwo)
```

**Steps**:

- **Step 4**: Created ON TOP of `feature/divisionByTwo`
- **Step 8**: Gets ALL code from main after other branches are merged
- **Final Integration**: Performs complete trapezoid calculation

## Git Workflow Journey

### Step 4: Initial Creation

```bash
# Start from feature/divisionByTwo branch
git checkout feature/divisionByTwo
git checkout -b feature/multiplication
```

### Step 8: Final Integration

```bash
# Get all updates from main branch
git checkout feature/multiplication
git rebase main
```

## How to Run This Branch

### After Step 4 (Initial)

1. **Switch to this branch**:

   ```bash
   git checkout feature/multiplication
   ```

2. **Compile and run**:

   ```bash
   javac TrapezoidCalculator.java
   java TrapezoidCalculator
   ```

3. **Expected Output**:

   ```bash
   Multiplication Test:
   divisionValue=2, h=3 -> Result: 6
   ```

### After Step 8 (Complete Integration)

```bash
Complete Trapezoid Calculator:
Given: a=4, b=6, h=5
Step 1 - Addition: 4 + 6 = 10
Step 2 - Division: 10 / 2 = 5  
Step 3 - Multiplication: 5 × 5 = 25
Final Trapezoid Area: 25
```

## Dependencies

This branch depends on:

### feature/divisionByTwo (Direct Parent)

- **Provides**: Division by 2 functionality
- **Usage**: Calculates (a+b)/2 part
- **Integration**: Direct inheritance through branch creation

### feature/addition (Through Rebasing)

- **Provides**: Addition of a and b
- **Usage**: Calculates a+b part  
- **Integration**: Received through main branch rebase in Step 8

### main (Final Integration)

- **Provides**: All merged features
- **Usage**: Complete trapezoid calculation capability
- **Integration**: Step 8 rebase operation

## Complete Workflow

1. **Step 4**: Created on top of `feature/divisionByTwo`
2. **Step 5**: `feature/addition` merged to main
3. **Step 6**: `feature/divisionByTwo` rebased with main  
4. **Step 7**: `feature/divisionByTwo` merged to main
5. **Step 8**: This branch gets all code from main (FINAL STEP)

## Testing

### Phase 1: Multiplication Only

- Test multiplication functionality independently
- Verify correct multiplication results
- Use mock division values for testing

### Phase 2: Complete Integration

- Test full trapezoid area calculation
- Verify all three operations work together

## Branch Status

- **Initial Implementation**: Complete (multiplication only)
- **Division Integration**: Inherited from parent branch
- **Addition Integration**: Awaiting Step 8 merge
- **Complete Solution**: Pending final integration

**Branch Author**: Divya Swarupa  

**Contact**:divyaswarupa@everest.engineering

**Assignment**: Challenge-2, Step 4 & Step 8