---
layout: research
category: Research
title: "Multiway Contingency Table Analysis"
subtitle: ": 다중 분할표 분석"
permalink: /researches/multi-cont
# image: recom.jpg
---

최근 경제학, 의학, 정치학 등 다양한 학문분야에서 다중 분할표에 대한 활용성 및 중요성이 매우 높아지면서, 이러한 형태의 자료 분석에 관한 여러 연구가 시도되고 있다. 이러한 다중 분할표 분석에서 주어진 제한 하에 다중 분할표로 부터의 샘플링은 조건부 추론을 위한 정확한 몬테카를로 p-value를 계산하는데 사용되어 질수 있다(Freeman and Halton, 1951; Agresti, 1992). 이러한 접근이 관심을 가지는 표의 수가 많다면 매우 적합하다. 하지만 점근적 방법의 유효성에 대한 논란은 가중되고 있다. 

이 분야의 보편적인 응용분야로 다중 대립유전자(allele)들의 Hardy-Weinberg equilibrium 검정이 있다. 여기서 어떤 대립유전자들은 극히 드물게 생성되고 그래서 표의 빈칸이 존재하는 자료를 만든다(Guo and Thompson, 1992). 다른 응용분야로 여러 위험인자를 가지는 그룹화된 case/control 자료의 모수 유의성 검정과 조건부 적합도 검정(Chen, Dinwoodie and MacGibbon, 2004), 그리고 Diaconis and Efron(1985)이 제안한 조건부 볼륨검정(Volume test)이 있다.

보다 일반적인 문제는 비음 정수 격자점으로부터 샘플링하는 데 있다. 이 분야에는 분할표를 포함하고 있고, 다른 응용 분야로 불완전한 자료에 대한  몬테카를로 EM(Expectation and Maximization) 알고리즘(Vardi, 1996)과 사후 분포의 베이지안 계산(Tebaldi and West, 1998)이 있다.

다중 분할표에 있어 주요 관심 분야는 관찰값에 대한 확률모형의 적합도 검정과 두 변수 이상의 독립성 검정 및 three-way 교차효과 검정 등이 있다. 이러한 분할표에서의 정확한 추론을 위해서는 분할표를 구성하는 모든 경우를 알 필요가 있다. 따라서 이러한 분할표에서의 정확한 추론을 위해 최대우도 추정법을 이용(Birch, 1963)하거나 Pearson의 카이제곱통계량을 분할(Beh and Davy, 1998)하는 연구를 하여 왔고, 근사시키는 방법으로 randomized 알고리즘(Barvinok et al.)을 개발하는 등 여러 가지 연구를 하여 왔다. 하지만 자료의 차원과 수가 증가함에 따라 이는 매우 불가능 한 것으로 알려져 왔음으로 이와 같은 문제를 해결하기 위하여 Markov chain Monte Carlo 알고리즘이 제안되어 오고 있다

(Bunea and Besag, 1996; Caffo and Booth, 2001).

Markov chain Monte Carlo(MCMC)는 어떤 제한을 가지는 표에서 랜덤 표본을 생성시키는데 많이 사용되고 있는 알고리즘이다. 일반적으로 이는 프로그램하기도 쉽고 많은 메모리를 사용할 필요도 없으며 응용 분야도 꽤 넓다. Diaconis and Sturmfels(1998)는 마코브 연쇄를 만드는데 필수적인 이동(move)의 특징들을 제시하였으나, 어떤 로그선형 모형에서 다중 분할표에서의 충분통계량이 가지고 있는 제한이 기약 마코브 연쇄(irreducible Markov chain)을 생성시키는데 어려움을 주고 있다. Diaconis and Sturmfels(1998)는 주어진 제한 하에 모든 표들을 연결하는 마코브 이동들을 생성시키는 방법들을 제시하였으나, 어떤 실용적인 면(예로 대량 로지스틱 회귀)에 있어 이러한 이동들은 불가능한 경우가 있다. 때때로 표의 일부 칸은 음수를 허용함으로써 위 이동들을 가능하게 할 수도 있다(Buena and Besag, 2000; Chen et al., 2004). 하지만 마코브 연쇄의 실행시간이 길어진 다는 단점이 있다. 일반적으로 이러한 마코브 연쇄의 실행시간을 판단하기란 쉽지가 않다. 그래서 마코브 연쇄는 일반적으로 디자인하기 힘들고, 정상성(Stationary)에 도달하는데 매우 오랜 시간이 걸리며, 정상성까지 걸리는 시간 또한 명확하게 결정할 수 없다. 

이를 극복하기 위해 Chen et al.(2005)은 sequential importance sampling(SIS) 알고리즘을 제안하였다. SIS의 개념은 최종 결합분포(proposal distribution)가 목표분포(target distribution)와 비슷해 지도록 분할표의 각 칸의 값들을 서로 서로 샘플하는 데에 있다. 따라서 SIS는 이용하기 쉽고, 정상성 분포로의 수렴을 보여 주었다. 하지만, SIS는 최종 결합분포로부터 표본들을 생성시키는 데에 있어 국소 트랩(local trap)의 문제점을 가지고 있다. 따라서 SIS 알고리즘은 기약 마코브 연쇄를 만드는 표본들을 생성시키는 매우 어렵다. 

본 연구에서는 국소 트랩의 문제점을 안고 있는 SIS 알고리즘을 극복하고자 Stochastic approximation Monte Carlo(SAMC; Liang, 2007)룰 이용한 알고리즘 개발을 목표로 한다. 

SAMC는 Wang-Landau(WL) 알고리즘을 개선한 고급 몬테카를로(Advanced Monte Carlo) 알고리즘으로 자기 조절능력(self adjusting)을 가지고 있어 국소 트랩을 쉽게 벗어나 원하는 분포의 최적(Optimization)의 값을 구할 수 있는 장점을 가지고 있다.

* 국제 논문 

Jung, B.C., So, S. and Cheon, S. (2014.03), Exact inference in contingency tables via Stochastic approximation Monte Carlo, Journal of the Korean Statistical Society(0.465), 43, 1, 31-45. 

Cheon, S., Liang, F., Chen, Y, Yu, K. (2014.07), Stochastic Approximation Monte Carlo Importance Sampling for Approximating Exact Conditional Probabilities, Statistics and Computing(1.429), 24, 4, 505-520. 

* 국내 논문

Cheon, S. (2012.10). Approximating Exact Test of Mutual Independence in Multiway Contingency Tables via Stochastic Approximation Monte Carlo. 응용통계 연구, 25, 5, 837-846.

전수영 (2013.02). Exact Inference for Three-way Interaction Effects. Journal of the Korean Data Analysis Society, 15, 1, 41-51.

전수영 (2019.10). 미디어자료 분할표 분석을 위한 정확추론. Journal of  the Korean Data Analysis Society, 21, 5, 2303-2312.

* 학회 발표

전수영. 미디어자료 분할표 분석을 위한 정확추론. 제7회 한국미디어패널 학술대회, 서울, 2019.10.25.