# Feature: Division By Two Implementation (Challenge-2)

This branch implements the division by 2 functionality for the trapezoid area calculation.

## Purpose

This branch is part of Challenge-2 and implements the division logic for the trapezoid area formula: **((a + b) / 2) × h**

## What This Branch Does

### Implementation Details

- **Function**: Divides any given value by 2
- **Input**: Integer value
- **Output**: Result divided by 2
- **Usage**: Convert (a + b) to (a + b)/2 in trapezoid formula

### Code Implementation

```java
public static double divisionByTwo(int value) {
    return value / 2;
}
```

## Test Cases

### Example from Assignment

- **Input**: additionValue = 6
- **Output**: 3.0
- **Note**: Assignment shows 6 → 4, but mathematically 6/2 = 3

### Additional Examples

## Branch Information

- **Branch Name**: `feature/divisionByTwo`
- **Parent Branch**: `main` (master)
- **Purpose**: Implement division by 2 for trapezoid calculation
- **Challenge**: Challenge-2, Step 2

## Git Workflow

This branch has a special role in Challenge-2's workflow:

```bash
main
├── feature/addition 
├── feature/divisionByTwo (this branch)
│   └── feature/multiplication (created ON TOP of this branch)
```

**Special Workflow Steps**:

- **Step 2**: Created this branch
- **Step 4**: `feature/multiplication` created ON TOP of this branch
- **Step 6**: This branch will be REBASED with main to get addition logic
- **Step 7**: This branch merged into main

## Rebasing Process (Step 6)

This branch will undergo rebasing:

```bash
# Before rebase: only has division logic
git checkout feature/divisionByTwo
# After rebase: will have addition + division logic
git rebase main
```

**Why Rebasing?**

- To get the addition logic from main branch
- To calculate (a+b)/2 using both addition and division

## How to Run This Branch

### Before Rebase

1. **Switch to this branch**:

   ```bash
   git checkout feature/divisionByTwo
   ```

2. **Compile and run**:

   ```bash
   javac TrapezoidCalculator.java
   java TrapezoidCalculator
   ```

3. **Expected Output**:

   ```bash
   Division by 2 Test:
   Input: 6 -> Output: 3
   Input: 10 -> Output: 5
   ```

### After Rebase (Step 6)

```bash
Division + Addition Test:
a=4, b=6 -> Addition: 10 -> Division: 5
Final (a+b)/2 = 5
```

## Assignment Requirements

### Challenge-2 Step 2 Requirements:

- Create branch called `feature/divisionByTwo`
- Implement division by 2 functionality
- Example: Input -> 6, Output -> 3 
- Prepare for multiplication branch creation on top

### Challenge-2 Step 6 Requirements:

- Rebase with main branch to get addition logic
- Use addition logic to calculate (a+b)/2
- Combine both addition and division functionalities

## Related Branches

### feature/multiplication

- **Relationship**: Created ON TOP of this branch
- **Purpose**: Will use this branch's division logic
- **Workflow**: Gets updated after this branch is rebased and merged

### feature/addition  

- **Relationship**: Will be integrated through rebasing
- **Purpose**: Provides addition logic needed for (a+b)/2
- **Integration**: Step 6 rebasing process

## Workflow Timeline

1. **Step 2**: Created this branch with division logic
2. **Step 4**: `feature/multiplication` created on top
3. **Step 5**: ⏳ `feature/addition` merged to main  
4. **Step 6**: ⏳ This branch rebased with main (gets addition logic)
5. **Step 7**: ⏳ This branch merged into main
6. **Step 8**: ⏳ `feature/multiplication` gets all updates

## Testing 

### Current Testing (Before Rebase)

- Test division functionality independently
- Verify correct division results
- Ensure no dependency issues

### After Rebase Testing

- Test combined addition + division logic
- Verify (a+b)/2 calculation works correctly
- Test integration with multiplication branch

**Branch Author**:M.Divyaswarupa 

**Contact**:divyaswarupa@everest.engineering 

**Assignment**:Challenge-2, Step 2 & Step 6