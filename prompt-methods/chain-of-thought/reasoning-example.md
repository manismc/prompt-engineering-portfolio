# Chain-of-Thought Reasoning Prompt Example — Advanced Financial Analysis

## Prompt

```plaintext
You are a seasoned financial analyst assistant. For every financial question, carefully analyze all relevant data and reasoning steps before providing a well-supported final answer.

Question: {input_question}

Please provide a detailed, step-by-step breakdown of your reasoning process, including all necessary calculations, assumptions, and financial principles applied. Conclude with a clear final recommendation or result.
````

## Purpose

This prompt is designed to elicit complex, structured reasoning in financial contexts where thorough analysis is essential. By requesting explicit, multi-step explanation of calculations, assumptions, and underlying principles, it ensures that the AI’s output is transparent, accurate, and professional.

It highlights the prompt engineer’s ability to craft instructions that guide the model through intricate problem-solving in a high-stakes domain.

## Example

**Input:**
"A company has a current stock price of \$150, expected annual dividend of \$5, and an expected growth rate in dividends of 4% per year. If the required rate of return is 8%, what is the intrinsic value of the stock using the Dividend Discount Model? Should an investor buy the stock at its current price?"

**Model output:**
Step-by-step reasoning:

1. **Identify the formula:** The Dividend Discount Model (DDM) for valuing a stock with constant growth is:

$$
P = \frac{D_1}{r - g}
$$

where:

* $P$ = intrinsic price of the stock
* $D_1$ = dividend expected next year
* $r$ = required rate of return
* $g$ = growth rate of dividends

2. **Calculate $D_1$:** Given the expected annual dividend is \$5, and dividends grow at 4%,

$$
D_1 = 5 \times (1 + 0.04) = 5.20
$$

3. **Plug values into the formula:**

$$
P = \frac{5.20}{0.08 - 0.04} = \frac{5.20}{0.04} = 130
$$

4. **Interpretation:** The intrinsic value of the stock is \$130 per share.

5. **Decision:** The current market price is \$150, which is higher than the intrinsic value (\$130). Therefore, based on the DDM, the stock appears overvalued.

6. **Recommendation:** Unless there are other qualitative factors or growth expectations not captured here, an investor should be cautious and might consider not buying at the current price.

**Final answer:** The intrinsic value is \$130. The stock is currently overvalued at \$150, so it is not recommended to buy at this price.

## Notes

* This prompt ensures the model explicitly applies financial formulas, shows intermediate calculations, and draws logical conclusions.
* Asking for assumptions and financial principles helps avoid black-box answers and makes the output auditable.
* The detailed reasoning supports both accuracy and transparency, critical in financial decision-making.
* This approach can be adapted for valuation, risk analysis, portfolio optimization, and other complex financial tasks.
