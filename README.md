# Bayesian Game Analysis on Indonesia's LQ45 Stock Market

## 📖 Background & Context

Financial markets, particularly emerging equity benchmarks such as Indonesia's **LQ45 Index**, operate in environments characterized by imperfect information, varying liquidity levels, and strategic interactions among market participants.

Traditional financial models often assume that all market participants are fully rational and possess symmetric information. In practice, however, financial markets consist of heterogeneous agents with different levels of information and analytical capabilities:

- **Informed Traders** – Institutional investors or sophisticated market participants with superior analytical resources.
- **Uninformed Traders** – Retail investors who primarily rely on delayed technical indicators and publicly available information.

Understanding the interaction between these two groups is essential for explaining real-world market behavior and deviations from classical financial theory.

---

## 🎯 Research Objectives

This study models strategic decision-making under uncertainty using a **Bayesian Game** framework. Under incomplete information, market participants form beliefs regarding the type of opponent they face and select strategies that maximize expected utility, resulting in a **Bayesian Nash Equilibrium (BNE)**.

The research focuses on two primary questions:

1. **Empirical Payoff Profiling**
   - How do effective payoffs and risk-return profiles differ between **Informed** and **Uninformed** market regimes when information premiums and risk penalties are incorporated?

2. **Equilibrium Convergence**
   - To what extent do actual trading strategies (derived from momentum indicators) align with or diverge from the theoretical **Bayesian Nash Equilibrium**?

---

## 💡 Theoretical & Practical Significance

This research combines **technical analysis** with **game-theoretic optimization** by integrating:

- Relative Strength Index (RSI)
- Trading Volume
- Bayesian Game Theory

The framework bridges the gap between formal economic theory and empirical market microstructure, providing insights into:

- Market efficiency
- Information asymmetry
- Trader behavior
- Risk dynamics
- Strategic decision-making in the Indonesian capital market

---

## 📊 Dataset Description

The dataset consists of daily observations from the Indonesian **LQ45 Index** with the following variables:

| Variable | Description |
|----------|-------------|
| **price ($P_t$)** | Adjusted Closing Price |
| **volume ($V_t$)** | Daily Transaction Volume |
| **return ($r_t$)** | Log Return: $r_t=\ln(P_t/P_{t-1})$ |
| **volatility ($\sigma_t$)** | Rolling 10-Day Standard Deviation |
| **rsi_lag ($RSI_{t-1}$)** | 14-Day Relative Strength Index (Lagged One Day) |

---

# 📈 Results & Discussion

## 1. Empirical Payoff Profile (Informed vs Uninformed)

### Key Findings

- The **median payoff** for both trader groups is centered close to zero.
- **Informed traders** exhibit substantially higher payoff dispersion.
- Positive payoff tails reach approximately **+0.20**, while downside losses extend beyond **−0.30**.
- **Uninformed traders** display a much narrower payoff distribution with fewer extreme outcomes.

### Interpretation

The results suggest that **information advantages do not necessarily translate into consistently higher returns**.

Instead:

- Higher information quality is associated with **greater payoff volatility**.
- Informed traders enjoy larger upside opportunities.
- They also bear significantly greater downside risk during adverse market conditions.

### Conclusion

> **Information premium comes with higher variance.**

Being informed increases the potential for excess returns but simultaneously exposes investors to larger losses, illustrating the classical **risk–reward tradeoff**.

---

## 2. Strategy Distribution Comparison (Actual vs Bayesian Nash Equilibrium)

### Key Findings

- The empirical market strongly favors the **Hold** strategy, with more than **1,200 observations**.
- The Bayesian Nash Equilibrium predicts substantially fewer **Hold** decisions (approximately **850**).
- Conversely, the theoretical model recommends more **Buy** and **Sell** actions than those observed in the actual market.

### Interpretation

Real-world investors demonstrate stronger trading inertia than predicted by the rational Bayesian model.

Possible explanations include:

- Transaction costs
- Market uncertainty
- Behavioral loss aversion
- Investor hesitation
- Factors not fully captured by RSI-based trading signals

### Conclusion

> **Empirical markets tend to under-trade relative to theoretical optimal behavior.**

Although the Bayesian Game framework provides a rational benchmark for strategic decision-making, actual investors display a pronounced tendency to delay trading, preferring to **Hold** rather than execute theoretically optimal **Buy** or **Sell** decisions.

---

# 📝 Overall Conclusions

The empirical analysis demonstrates that:

- **Informed traders** experience higher payoff variability, reflecting both larger upside opportunities and greater downside exposure.
- Information advantages create **risk premiums** rather than guaranteed superior returns.
- Actual investor behavior deviates from the predictions of **Bayesian Nash Equilibrium**, primarily due to behavioral and market frictions.
- The Bayesian Game framework serves as a useful theoretical benchmark but does not fully capture the complexity of real-world trading behavior.

Overall, this study highlights the importance of combining **game theory**, **behavioral finance**, and **technical market indicators** to better understand strategic interactions in emerging financial markets.
