# Instruction Prompt Example — Complex Document Information Extraction

## Prompt

```plaintext
You are an expert data extraction assistant. Given a financial report text, carefully extract the following information:

1. Company Name  
2. Report Date  
3. Total Revenue (in USD)  
4. Net Income (in USD)  
5. Earnings Per Share (EPS)  
6. Any forward-looking statements or guidance mentioned  

Provide your answers in a structured JSON format. If any information is missing, indicate it as null.

Financial Report Text:  
"{input_text}"
````

## Example

**Input:**

```
Acme Corp announced its Q2 2025 earnings on July 15, 2025. The company reported a total revenue of $5.4 billion, with a net income of $870 million. Earnings per share stood at $1.25. Management expressed confidence in reaching a 10% growth target for the next fiscal year despite economic uncertainties.
```

**Model output:**

```json
{
  "Company Name": "Acme Corp",
  "Report Date": "July 15, 2025",
  "Total Revenue": 5400000000,
  "Net Income": 870000000,
  "Earnings Per Share": 1.25,
  "Forward-Looking Statements": "Management expressed confidence in reaching a 10% growth target for the next fiscal year despite economic uncertainties."
}
```
