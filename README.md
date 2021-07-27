# [Federated Stochastic Gradient Langevin Dynamics](https://www.auai.org/uai2021/pdf/uai2021.652.pdf)
This repository contains sample code describing some methods and experiments described in 

Khaoula El Mekkaoui, Diego Mesquita, Paul Blomstedt, Samuel Kaski
**Federated Stochastic Gradient Langevin Dynamics** [[UAI]](https://www.auai.org/uai2021/pdf/uai2021.652.pdf), [[Arxiv]](https://arxiv.org/abs/2004.11231)

**Abstract:**

Stochastic gradient MCMC methods, such as stochastic gradient Langevin dynamics (SGLD), employ fast but noisy gradient estimates to enable large-scale posterior sampling. Although we can easily extend SGLD to distributed settings, it suffers from two issues when applied to federated non-IID data. First, the variance of these estimates increases significantly. Second, delaying communication causes the Markov chains to diverge from the true posterior even for very simple models. To alleviate both these problems, we propose _conducive gradients_, a simple mechanism that combines local likelihood approximations to correct gradient updates. Notably, conducive gradients are easy to compute, and since we only calculate the approximations once, they incur negligible overhead. We apply conducive gradients to distributed stochastic gradient Langevin dynamics (DSGLD) and call the resulting method federated stochastic gradient Langevin dynamics (FSGLD). We demonstrate that our approach can handle delayed communication rounds, converging to the target posterior in cases where DSGLD fails. We also show that FSGLD outperforms DSGLD for non-IID federated data with experiments on metric learning and neural networks.

## Contact

* Khaoula El Mekkaoui(corresponding author), [Khaoula.elmekkaoui@aalto.fi](mailto:khaoula.elmekkaoui@aalto.fi)
* Diego mesquita, [diego.mesquita@aalto.fi](mailto:diego.mesquita@aalto.fi)
* Paul Blomstedt [paul.blomstedt@f-secure.com](mailto:paul.blomstedt@f-secure.com)
* Samuel Kaski [samuel.kaski@aalto.fi](mailto:samuel.kaski@aalto.fi)

Work done in the [Probabilistic Machine Learning research group](https://research.cs.aalto.fi/pml/) at [Aalto University](https://www.aalto.fi/en).
