---
layout: research
category: Research
title: "Change-point and Regime Switching Analysis"
subtitle: ": 변환점 분석"
permalink: /researches/change-point
# image: recom.jpg
---

경제학, 금융학, 의학 및 지리학 등 여러 분야의 자료에서 요즈음 변환 시점에 관심이 많아 졌고, 이 분야에 베이지안 방법 또한 많이 연구되어져 왔다. 

지금까지 개발된 변환점 모형은 많은 모수를 포함하고 있다. 이와 같이 모수의 수가 많을 경우 표본들의 분포가 매우 복잡한 현상을 가지는데, 이때 그 분포에 여러 최빈수가 있는 경우가 흔하게 발생한다. 이러한 경우, 많은 연구자들에 의해 알려졌듯이 Metropolis-Hastings(MH, Metropolis et al, 1953; Hastings, 1970) 알고리즘과 Gibbs 샘플러(Casella and George, 1992; Tanner, 1993)와 같은 전통적인 MCMC방법은 샘플들을 임의의 한 최빈수근처에서 계속 추출하여 전체공간의 최소값(Global Minima)을 구하지 못하는 국소 트램(Local Trap)의 문제점을 가지게 된다. 

본 연구는 다양한 변환점 모형의 효율적인 추론을 위해 Wang-Landau (2001) 알고리즘을 개선한 Adaptive Monte Carlo 알고리즘인 SAMC 알고리즘을 이용한 연구를 목표로 한다. 

* 국제 논문

Cheon, S. and Kim, J. (2010.02). Multiple Change-point Detection of Multivariate Mean Vectors with Bayesian Approach, Computational Statistics and Data  Analysis(1.028), 54, 2, 406-415. 

Kim, J. and Cheon, S. (2010.06). Bayesian Multiple Change-point Estimation with Annealing Stochastic Approximation Monte Carlo, Computational Statistics (0.276), 25, 2, 215-239. 

Kim, J. and Cheon, S. (2010.07). Bayesian Multiple Change-point Estimation Using SAMC, Proceedings of the Tenth Islamic Countries Conference on Statistical Sciences (ICCS-X), Volume II, The Islamic Countries Society of Statistical  Sciences, Lahore: Pakistan, 823-830.

Kim, J. and Cheon, S. (2010.09). A Bayesian regime-switching time series model, Journal of Time Series Analysis(0.761), 5, 31, 365-378.

Cheon, S. and Kim, J. (2014.07), A Bayesian structural change analysis via Stochastic Approximation Monte Carlo and Gibbs Sampler. Journal of Statistical Computation and Simulation(0.629), 84, 7, 1444-1470.

Kim, J. and Cheon, S. (2014.10), Stochastic approximation Monte Carlo Gibbs sampling for structural change inference in a Bayesian heteroscedastic time series model. Journal of Applied Statistics(0.449), 41, 10, 2157-2177. 

Lim, H-K., Lee, J. and Cheon, S. (2017.01), Stochastic approximation Monte  Carlo EM for change point analysis, Journal of Statistical Computation and Simulation(0.767), 87, 1, 69-87.   

Kim, J, Cheon, S. and Jin, Z. (2020.03), Bayesian multiple change-points estimation for hazard with censored survival data from exponential distributions, Journal of the Korean Statistical Society(0.557), 49, 1, 15-31.

* 국내 논문

Kim, J. and Cheon, S. (2006.12). Bayesian Multiple Change-point Estimation in Normal with EMC. 한국통계학회논문집, 13, 3, 621-633.

Kim, J. and Cheon, S. (2009.05). Parametric Tests and Estimation of Mean Change in Discrete Distributions. 한국통계학회논문집, 16, 3, 511-518.

Kim, J. and Cheon, S. (2009.08). Multiple change-point estimation of air pollution mean vectors. 응용통계연구, 22, 4, 687-695.

Cheon, S. and Lee, H.C. (2011.04). Bayesian Regime-switching Analysis via Stochastic Approximation Monte Carlo, Journal of the Korean Data Analysis Society, 13, 2. 599-609.

전수영, 유문성 (2012.03). 소량자료를 위한 베이지안 다중변환점모형. 한국통계학회 논문집, 19, 2, 237-246.

Cheon, S. and Yu, W. (2012.12). Bayesian multiple change-point estimation of multivariate mean vectors for small data. 응용통계 연구, 25, 6, 999-1008.

Kim, J and Cheon, S. (2013.11). Bayesian Multiple Change-point Estimation and Segmentation. Communications for Statistical Applications and Methods, 20, 6, 439-454.

전수영 (2019.04). Evolutionary Monte Carlo EM for Change Point Analysis. Journal of the Korean Data Analysis Society, 21, 2, 559-569.