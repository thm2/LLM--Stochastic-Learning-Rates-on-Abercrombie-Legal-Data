# LLM--Stochastic-Learning-Rates-on-Abercrombie-Legal-Data

This project experimentally couples LLMs and stochastic learning rates, see [1](https://arxiv.org/pdf/2110.10710.pdf) or [work 2](https://ieeexplore.ieee.org/abstract/document/9809984) for details.

The experiments will be conducted on legal data and tasks of [LegalBench](https://github.com/HazyResearch/legalbench) using GPT-2. In specific, the task will be to classify a particular mark (e.g. a name for a product or service) correctly. Per the [Abercrombie Task](https://github.com/HazyResearch/legalbench/tree/main/tasks/abercrombie), a particular mark (e.g. a name for a product or service) is only eligible for trademark protection if it is considered to be distinctive. In assessing whether a mark is distinctive, lawyers and judges follow the framework set out in the case Abercrombie & Fitch Co. v. Hunting World, Inc., which enumerates 5 categories of distinctiveness. These categories characterize the relationship between the dictionary definition of the term used in the mark, and the service or product it is being attached to.

The goal is to compare the performance of various algorithms (e.g. ADAM, ADAMW, SGD, etc.) when using stochastic learning rates versus the traditional deterministic learning rates. The results demonstrate that algorithms equipped with a stochastic learning rate yield better performance even when using legal and comparable, if not better testing performance. Even though the training data is disproportionally fewer than the testing data, the algorithms equipped with a stochastic learning rate were able to outperform their deterministic-learning-rate counterparts:


<img width=“964” alt=“java 8 and prio java 8  array review example” src=“https://github.com/thm2/LLM--Stochastic-Learning-Rates-on-Abercrombie-Legal-Data/tree/main/preliminary_results/ADAMW/%20slro_losses.png”>






