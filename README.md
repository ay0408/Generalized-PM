# Generalized Piecewise Mechanism (GPM) and Privacy-Optimized GPM for Collecting Multidimensional Data

In "Theoretical Comparison" folder, we compared our GPM with the existing methods in terms of the variance of collected private values.

"Privacy Guarantees" folder contains the codes for evaluating the achieved privacy guarantees for the entire (multidimensinal) data, when the privacy level regarding each attribute information was respectively given.

"Accuracy" folder provides the codes for evaluating the utility of our method using simulaton data and real data (from [IPUMS International](https://international.ipums.org/international/)), when the privacy budget for the entire data was given. (Our method allows more of the privacy budget to be distributed for each $\epsilon_i$ and provides a higher accuracy.)

In "RunTime.ipynb", we measured the run time to solve the minimization problem for obtaining the optimized $P_v$ in our enhanced GPM.


## Future Directions

・ Developing specialized methods for each analysis purpose (e.g., mean estimation and classification) while considering a hybrid mechanism with reference to existing studies [[Wang et al., 2019](https://doi.org/10.1109/ICDE.2019.00063), [Zhao et al., 2021](https://doi.org/10.1109/JIOT.2020.3037194)].  
(Note: The discussion of PM-OPT in Zhao et al.'s paper focused only on worst-case variance and proposed an "optimal" PM. However, that was not enough; for example, a smaller best-case variance is achieved by the original PM than the PM-SUB when $\epsilon$ is small. In this study, we present a generalized PM that is more concise (even for the subsequent discussion of enhanced GPM) than PM-OPT and compare it with existing methods theoretically in more detail. Indeed, the GPM achieves a truly smaller variance than the original PM for all $\epsilon$ and $t$.)

・ When the number of dimensions exceeds about $15$, the run time of our enhanced GPM will be out of a practical time frame (See Section V.C in our paper). To address this issue, more efficient algorithms or heuristic methods will be required. (cf. [Yamamoto and Shibuya, 2024](https://arxiv.org/abs/2402.07584))

・ Developing a method that allows random sampling or dimensionality reduction while setting the privacy level of each attribute information.

## Note

For details of our methods and discussion, please see our paper entitled "Generalization and Enhancement of Piecewise Mechanism for Collecting Multidimensional Data" presented at IEEE SpaCCS 2024.

### Contact
Akito Yamamoto

Division of Medical Data Informatics, Human Genome Center,

the Institute of Medical Science, the University of Tokyo

a-ymmt@ims.u-tokyo.ac.jp
