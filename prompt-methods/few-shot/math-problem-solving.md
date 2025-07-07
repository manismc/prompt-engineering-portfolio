# Few-Shot Math Problem Solving Prompt — Complex Examples

## Prompt

```plaintext
Solve the following math problems step-by-step. Show all your calculations and explain your reasoning clearly.

Example 1:  
Q: Solve for \(x\) in the equation \(2x + 3 = 11\).  
A:  
Step 1: Subtract 3 from both sides: \(2x = 11 - 3 = 8\).  
Step 2: Divide both sides by 2: \(x = \frac{8}{2} = 4\).  
Final answer: \(x = 4\).

Example 2:  
Q: A rectangle has a length of 10 cm and a width that is 4 cm shorter than its length. Find the area of the rectangle.  
A:  
Step 1: Calculate the width: \(10 - 4 = 6\) cm.  
Step 2: Calculate the area: length \(\times\) width \(= 10 \times 6 = 60\) cm\(^2\).  
Final answer: \(60\) cm\(^2\).

Example 3:  
Q: What is the derivative of \(f(x) = 3x^2 + 5x - 4\)?  
A:  
Step 1: Derivative of \(3x^2\) is \(6x\) (using power rule).  
Step 2: Derivative of \(5x\) is \(5\).  
Step 3: Derivative of constant \(-4\) is \(0\).  
Step 4: Combine: \(f'(x) = 6x + 5\).  
Final answer: \(f'(x) = 6x + 5\).

Now solve this problem:  
Q: {input_question}  
A:
````

## Purpose

This few-shot prompt provides clear, detailed examples covering algebra, geometry, and calculus. It trains the model to approach math problems methodically by breaking down each step logically and explaining the rationale, ensuring accuracy and interpretability.

## Example

**Input:**
"A circle has a radius of 7 cm. Calculate its circumference and area. (Use $\pi \approx 3.14$)"

**Model output:**
Step 1: Calculate the circumference using the formula $C = 2\pi r = 2 \times 3.14 \times 7 = 43.96$ cm.
Step 2: Calculate the area using the formula $A = \pi r^2 = 3.14 \times 7^2 = 3.14 \times 49 = 153.86$ cm$^2$.
Final answers: Circumference = 43.96 cm, Area = 153.86 cm$^2$.
