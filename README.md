# Metrics-simulation

This repository contains code and knitted documents of simulations I worked on as part of Econ metrics classes at UO.

# Description of DGPs

## [Measurement Error in DGP](code/metrics_khurana_PS2_05122024.Rmd)

DGP: $y = \alpha+ \beta_x + \epsilon$

$\epsilon$ is described as following in different DGPs:

-   Homoskedastic disturbance
-   Heteroskedastic error
-   Classical measurement error in `x`
-   Non-classical measurement error in `x`: heteroskedastic noise
-   Non-classical measurement error in `x`: correlated with `x`

## [Different instruments in IV estimation strategy](code/metrics_khurana_final-home_06132024.qmd)

DGP: $Y_i = \alpha + \tau_{g(i)} D_i + \gamma Z_{3i} + w_i + u_i$

We have three possible instruments for $D$. Each is binary (with 50% chance of being equal to $1$) and affects a specific group.

-   $Z_1=1$ increases the probability of treatment for group $a$ from 0.1 to 0.5;
-   $Z_2=1$ increases the probability of treatment for group $b$ from 0.3 to 0.6;
-   $Z_3=1$ increases the probability of treatment for group $c$ from 0.2 to 0.8.
-   For group $d$, the probability of treatment is 0.7.

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
