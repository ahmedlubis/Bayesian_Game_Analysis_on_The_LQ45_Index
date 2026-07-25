Background & Context
Financial markets, particularly emerging equity benchmarks such as Indonesia's LQ45 Index, operate in environments characterized by imperfect information, varying liquidity levels, and strategic interactions among market participants. Traditional financial models frequently rely on the assumption of fully rational agents possessing symmetric information. In empirical reality, however, market dynamics are shaped by interactions between heterogeneous traders—specifically, Informed agents (such as institutional investors with superior analytical capacity) and Uninformed agents (such as retail traders relying on lagging technical signals).

Problem Statement & Research Objectives
To model strategic decision-making under uncertainty, this study employs a Bayesian Game framework. In an incomplete information setting, market participants form ex-ante beliefs regarding the regime or "type" of opponent they face and optimize their choices accordingly to achieve a Bayesian Nash Equilibrium (BNE).

This research addresses two main objective questions:
1. Empirical Payoff Profiling: How do effective payoffs and risk-return profiles differ between Informed and Uninformed market regimes when risk penalties and information premia are introduced?
2. Equilibrium Convergence: To what extent do actual strategy choices (driven by momentum indicators) align with or diverge from theoretical Bayesian Nash Equilibrium predictions?

Theoretical & Practical Significance
By integrating technical indicators (RSI momentum and transaction volume) with formal game-theoretic optimization, this thesis bridges the gap between pure strategic economic theory and empirical market microstructure. It provides actionable insights into market efficiency, trader inertia, and risk dynamics in the Indonesian capital market.

Dataset Description
1. price (Pt​) : Adjusted Closing Price (Adt​).
2. volume (Vt​) : Daily Transaction Volume (Vot​).
3. return (rt​) : rt​=ln(Pt​/Pt−1​).
4. volatility (σt​) : Rolling 10-day Standard Deviation.
5. rsi_lag (RSIt−1​) : 14-day Relative Strength Index (lagged 1 day).

The conclusions

Plot 1: Empirical Payoff Profile (Informed vs Uninformed)
Key Findings
Median Payoff: Both group types (Informed and Uninformed) have median payoffs centered very close to zero.

Variance & Tail Risk (Outliers): The Informed group displays significantly higher dispersion (wider spread of red outlier points), reaching upside gains near +0.20 and downside losses past -0.30. The Uninformed group has a narrower distribution with fewer extreme outliers.

Core Conclusion
Information Premia Come with Variance: Being "Informed" (proxied by higher trading volume days) does not guarantee consistently higher baseline returns. Instead, high-volume periods subject investors to higher payoff volatility and asymmetric risk exposure.

Risk-Reward Tradeoff: Informed traders capture larger upside payoffs (positive tail), but they are simultaneously exposed to severe downside potential during market drops.

Plot 2: Strategy Distribution Comparison (Actual vs Predicted BNE)
Key Findings
Hold Strategy: Actual market behavior (action, dark blue) shows a heavy bias toward Hold (around 1,200+ instances), whereas the theoretical model (BNE_Equilibrium, yellow) predicts fewer Hold decisions (~850).

Buy & Sell Strategies: The actual market shows lower execution frequencies for Buy and Sell compared to what the theoretical Bayesian Nash Equilibrium model prescribes.

Core Conclusion
Status Quo Bias / Inertia: Real-world market participants exhibit stronger inertia or reluctance to trade than the theoretical model predicts. While the BNE model dynamically dictates taking action (Buy or Sell) whenever expected utilities outweigh holding penalties, actual traders display a higher tendency to wait (Hold), likely driven by transaction costs, uncertainty, or behavioral loss aversion not fully captured by simple RSI triggers.

Model Divergence: The Bayesian game framework provides a solid baseline for rational decision-making, but empirical trading patterns show under-trading relative to theoretical optimality.

Synthesis Statement:
"The Bayesian game framework demonstrates that while informed trading creates opportunities for extreme upside payoffs, it carries substantial volatility. Furthermore, empirical trader behavior exhibits a significant conservative bias—holding far more frequently than the optimal Bayesian Nash Equilibrium suggests—pointing to real-world friction and risk aversion in the LQ45 market."
