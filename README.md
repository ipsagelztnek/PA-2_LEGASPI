## PA2 - NumPy Problems  

## Problem 1: Normalization  

### What it does  
- Creates a 5x5 array with random floating-point numbers between 0 and 1.  
- Calculates the mean and the standard deviation of the array.  
- Normalizes the array using the formula:  

  \[
  Z = \frac{X - \text{mean}}{\text{std}}
  \]  

- Saves the normalized array as **X_normalized.npy**.  

### Key points in the code  
1. `np.random.random((5, 5))` → generates the 5x5 array.  
2. `np.average(X)` → gets the mean.  
3. `np.sqrt(np.mean((X - mean_value) ** 2))` → computes the standard deviation.  
4. `(X - mean) / std` → performs normalization.  
5. `np.save("X_normalized.npy", Z)` → saves the result.  

### Output  
- Prints the original array.  
- Shows the mean and standard deviation.  
- Displays the normalized array.  
- Creates a file: `X_normalized.npy`.  

---

## Problem 2: Divisible by 3  

### What it does  
- Creates an array of squared numbers from 1 to 100.  
- Reshapes it into a 10x10 matrix.  
- Finds all numbers that are divisible by 3 using Boolean indexing.  
- Saves the filtered results as **div_by_3.npy**.  

### Key points in the code  
1. `np.arange(1, 101) ** 2` → creates squares of numbers 1–100.  
2. `.reshape(10, 10)` → reshapes the array into a 10x10 matrix.  
3. `A[A % 3 == 0]` → extracts only numbers divisible by 3.  
4. `np.save("div_by_3.npy", div_by_3)` → saves the result.  

### Output  
- Prints the 10x10 matrix of squared numbers.  
- Displays the list of numbers divisible by 3.  
- Creates a file: `div_by_3.npy`.  

---

## How to Run  

1. Install NumPy if not installed:  
   ```bash
   pip install numpy

