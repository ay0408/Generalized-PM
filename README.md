# Generalized Piecewise Mechanism (GPM) and Privacy-Optimized GPM for Collecting Multidimensional Data

In "Theoretical Comparison" folder, we compared our GPM with the existing methods in terms of the variance of collected private values.

"Privacy Guarantees" folder contains the codes for evaluating the achieved privacy guarantees for the entire (multidimensinal) data, when the privacy level regarding each attribute information was respectively given.

"Accuracy" folder provides the codes for evaluating the utility of our method using simulaton data and real data (from [IPUMS International](https://international.ipums.org/international/)), when the privacy budget for the entire data was given. (Our method allows more of the privacy budget to be distributed for each $\epsilon_i$ and provides a higher accuracy.)

In "RunTime.ipynb", we measured the run time to solve the minimization problem for obtaining the optimized $P_v$ in our enhanced GPM.


## Future Directions

・ Developing specialized methods for each analysis purpose, such as mean estimation and classification, with reference to the existing study [[Wang et al., 2019](https://doi.org/10.1109/ICDE.2019.00063)], while considering a hybrid mechanism.

・ Developing a method that allows random sampling or dimensionality reduction while setting the privacy level of each attribute information.

## Note

For details of our methods and discussion, please see our paper entitled "Generalization and Enhancement of Piecewise Mechanism for Collecting Multidimensional Data".

### Contact
Akito Yamamoto

Division of Medical Data Informatics, Human Genome Center,

the Institute of Medical Science, the University of Tokyo

a-ymmt@ims.u-tokyo.ac.jp
