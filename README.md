# Feature: Addition Implementation (Challenge-2)

This branch implements the addition functionality for calculating the sum of trapezoid's parallel sides (a + b).

## Purpose

This branch implements the addition logic that will be used in the trapezoid area calculation formula: **((a + b) / 2) × h**

## What This Branch Does

### Implementation Details

- **Function**: Adds two values (a and b)
- **Input**: Two integers representing parallel sides of trapezoid
- **Output**: Sum of the two values
- **Usage**: Will be integrated with division and multiplication features

### Code Implementation

```java
public static int addition(int a, int b) {
    return a + b;
}
```

## Test Cases

### Example 1

- **Input**: a = 2, b = 3
- **Output**: 5
- **Usage**: First step in calculating ((2+3)/2) × h

### Example 2  

- **Input**: a = 4, b = 6
- **Output**: 10
- **Usage**: First step in calculating ((4+6)/2) × h

## Branch Information

- **Branch Name**: `feature/addition`
- **Parent Branch**: `main` (master)
- **Purpose**: Implement addition of trapezoid parallel sides
- **Challenge**: Challenge-2, Step 3

## Git Workflow

This branch is part of Challenge-2's complex workflow:

```bash
main
├ feature/addition (this branch)
├ feature/divisionByTwo  
 |  feature/multiplication
```

**Workflow Step**: Step 3 of Challenge-2

- Created after `feature/divisionByTwo` 
- Will be merged to main in Step 5
- Will be rebased into `feature/divisionByTwo` in Step 6

## How to Run This Branch

1. **Switch to this branch**:

   ```bash
   git checkout feature/addition
   ```

2. **Compile and run**:

   ```bash
   javac TrapezoidCalculator.java
   java TrapezoidCalculator
   ```

## Assignment Requirements

### Challenge-2 Step 3 Requirements:

- Create branch called `feature/addition`
- Implement addition of a and b values
- Example: Input -> a=2, b=3, Output -> 5
- Prepare for integration with other features

## Integration Points

This addition feature will be used by:

1. **feature/divisionByTwo**: After rebasing, will use addition to calculate (a+b)/2
2. **feature/multiplication**: Will use the complete (a+b)/2 result for final calculation
3. **main branch**: Final integrated solution

## Next Steps

1. **Step 5**: This branch will be merged into main
2. **Step 6**: Addition logic will be rebased into `feature/divisionByTwo`
3. **Step 8**: Final integration in `feature/multiplication`

## Testing Instructions

### Manual Testing

1. Switch to this branch
2. Run the calculator
3. Verify addition results match expected outputs
4. Test with different a, b values

## Branch Status

- **Implementation**: Complete
- **Testing**: Passed
- **Merge Status**: Ready for Step 5 merge
- **Rebase Status**: Will be rebased in Step 6

**Branch Author**: Divya Swarupa  

**Contact**:divyaswarupa@everest.engineering  
