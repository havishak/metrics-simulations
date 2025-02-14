# Metrics-simulation

This repository contains code and knitted documents of simulations I worked on as part of Econ metrics classes at UO.

# Description of DGPs

## [Positive selection into treatment](code/metrics_khurana_A1_01202025.Rmd)

DGP: $y = f(x_{1}, x_{2}, T),$ and $Z = 1 + a_1x_1 + a_2x_2$ determines the probability each individual gets treated, such that $$Pr[T=1] = \frac{1}{1+e^{-Z}}~.$$

## [Difference in Population Variance of Control and Treatment Group](code/metrics_khurana_A5_02112025.Rmd)

DGP: $Y_C \sim \mathcal{N}(0, \mu_C); Y_T \sim \mathcal{N}(1, \mu_T); \mu_T > \mu_C$, and $y = f(T)$

## [DiD estimates with other](code/metrics_khurana_A5_02042025.Rmd)

DGP: $Y = \beta_1*X + \beta_2*Tr + \beta_3*X*Tr + \beta_4*T + beta_5*T*Tr + \beta_6*Cx + \epsilon_i + \epsilon_t + \epsilon_c + \epsilon_it$

## [Comparing DiD and TWFE estimates with different error structure](code/metrics_khurana_A3_02142025.Rmd)

DGP: $Y = \beta_1*X + \beta_2*Tr + \beta_3*X*Tr + \epsilon_it$

$Y = \beta_1*X + \beta_2*Tr + \beta_3*X*Tr + \epsilon_it + \epsilon_i$

$Y = \beta_1*X + \beta_2*Tr + \beta_3*X*Tr + \epsilon_it + \epsilon_t$

$Y = \beta_1*X + \beta_2*Tr + \beta_3*X*Tr + \epsilon_it + \epsilon_i + \epsilon_t$
