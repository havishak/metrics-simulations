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

<img src="figures/A1_figure.png" width="800">

## [Difference in Population Variance of Control and Treatment Group](code/metrics_khurana_A5_02112025.Rmd)

DGP: $Y_C \sim \mathcal{N}(0, \mu_C); Y_T \sim \mathcal{N}(1, \mu_T); \mu_T > \mu_C$, and $y = f(T)$

<img src="figures/A2_df_fig.png" width="800">
<img src="figures/A2_estimate_fig.png" width="800">

## [DiD estimates with other](code/metrics_khurana_A5_02112025.Rmd)

DGP: $Y = \beta_1X + \beta_2Tr + \beta_3XTr + \beta_4T + beta_5TTr + \beta_6Cx + \epsilon_i + \epsilon_t + \epsilon_c + \epsilon_{it}$

<img src="figures/A3_estimate_fig.png" width="800">
<img src="figures/A3_std_error_estimate.png" width="800">

## [Comparing DiD and TWFE estimates with different error structure](code/metrics_khurana_A3_02142025.Rmd)

DGP: $Y = \beta_1X + \beta_2Tr + \beta_3XTr + \epsilon_{it}$

$Y = \beta_1X + \beta_2Tr + \beta_3XTr + \epsilon_{it} + \epsilon_i$

$Y = \beta_1X + \beta_2Tr + \beta_3XTr + \epsilon_{it} + \epsilon_t$

$Y = \beta_1X + \beta_2Tr + \beta_3XTr + \epsilon_{it} + \epsilon_i + \epsilon_t$

<img src="figures/A5_estimate_fig.png" width="800">
<img src="figures/A5_std_error_estimate_fig.png" width="800">

## [Event Studys TWFE with different violations](code/metrics_khurana_A6-event-studies_02212025.Rmd)

Estimation: $y_{it} = \alpha + \sum_{t \ne T-1}\beta_t(T_{it}=1) + \lambda_{i} + \mu_{t} + e_{it}$

Violations:

-   Non-parallel trends
-   Parallel pre-trends and non-parallel post-trends
-   Ashenfelter dip
-   Anticipated treatment
-   Unbalanced data
-   Staggered treatment
-   Heterogeneous treatment

<img src="figures/A6_df_fig.png" width="800">
<img src="figures/A6_estimate_fig.png" width="800">


## [Comparing DiD and TWFE standard-error estimates with different clustering specification](code/metrics_khurana_A7-se_20250225.Rmd)

DGP: $Y = \beta_1X + \beta_2Tr + \beta_3XTr + \epsilon_{it} + \epsilon_i + \epsilon_t$

Clustering Specifications:

- iid
- ~i
- ~t
~ i+t

<img src="figures/A7_std_error_estimate_fig.png" width="800">