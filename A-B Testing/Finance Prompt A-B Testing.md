# Prompt A/B Testing Example: AI Financial Advisor for Personalized Investment Recommendations

---

### Context:

We are building an AI-powered financial advisor designed to provide personalized investment recommendations to retail investors with varying risk tolerances, financial goals, and market knowledge.

---

### Objective:

Compare two prompt strategies to determine which yields more accurate, personalized, and trustworthy investment advice, improving user confidence and engagement.

---

### Prompt Variants:

---

**Prompt A: Rule-Based, Risk-Centric Prompt**

* **Description:**
  This prompt explicitly incorporates risk profiles and regulatory constraints. It guides the AI to prioritize conservative, compliant advice emphasizing risk management.

* **Prompt Structure:**

```
You are a licensed financial advisor providing investment advice. Consider the client's risk tolerance: {risk_tolerance} (low, medium, high), investment horizon: {investment_horizon}, and financial goals: {financial_goals}. Provide clear, compliant, and risk-aware investment recommendations focusing on portfolio diversification and capital preservation.

Client profile: {client_profile}
Market conditions: {market_conditions}

Advice:
```

* **Features:**

  * Explicit risk and compliance emphasis
  * Focus on conservative, structured guidance
  * Includes regulatory disclaimers in responses

---

**Prompt B: Behavioral Finance-Informed, Client-Centered Prompt**

* **Description:**
  This prompt integrates behavioral finance principles to address cognitive biases, emotional factors, and client psychology. The AI advisor adopts a conversational, trust-building tone tailored to client's behavioral profile.

* **Prompt Structure:**

```
You are a trusted financial advisor helping a client with the following profile: {client_profile}. Acknowledge their behavioral biases, emotions, and preferences. Guide them gently towards investment decisions aligned with their long-term goals: {financial_goals}. Use empathetic, transparent language to build trust and explain market risks and opportunities clearly.

Current market outlook: {market_conditions}

Recommendation:
```

* **Features:**

  * Behavioral finance framing
  * Empathy and trust-building language
  * Tailored explanations addressing biases like loss aversion

---

### Testing Plan:

* **Population:** 1,000 retail investors across various demographics and investment experience levels.
* **Study Design:** Randomized controlled trial with stratification by risk tolerance and investment experience.
* **Data Collection:**

  * AI-generated recommendations stored and analyzed.
  * User feedback via surveys rating clarity, trustworthiness, and satisfaction.
  * Behavioral follow-up: tracking if users follow recommendations via simulated portfolios.

---

### Evaluation Metrics:

* **Advice Quality:**

  * Expert financial advisor ratings on accuracy, compliance, and suitability.
  * Alignment with client risk profiles.

* **User Perception:**

  * Trust and confidence scores.
  * Perceived clarity and empathy ratings.

* **Behavioral Outcomes:**

  * Simulated adherence to recommendations.
  * Changes in risk-adjusted portfolio performance.

* **Operational Metrics:**

  * Response length and complexity (balance information and brevity).
  * Frequency of disclaimers and risk warnings.

---

### Analysis Approach:

* Multivariate regression to analyze impact of prompt on trust and adherence.
* Sentiment analysis of user feedback comments.
* Subgroup analysis by investor sophistication and risk tolerance.
* A/B comparison with significance testing and effect size estimation.

---

### Challenges & Mitigations:

* **Balancing regulatory compliance with user engagement:** Embed disclaimers without overwhelming users.
* **Measuring long-term behavioral impact:** Use simulations and proxies for adherence.
* **Handling diverse user profiles:** Incorporate dynamic prompt templating.
