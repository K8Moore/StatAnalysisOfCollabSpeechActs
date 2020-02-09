# Hotelling T-test
Code used to perform statistical analysis of speech acts from collaborative conversations. 

Data Summary:
The data in this study are continuous count variables. Each speech act is a vector of the number of times raters counted that speech act in a conversation. The speech acts have been summed across dyads and partitions by condition. Vector means and standard deviations are displayed in Table 2.
There is large variability in these data (see Figure 1). The generalized variance and total variance are extremely high (Determinate = 1.55x101  2 , Trace = 1129.9). This high variability is in part due to the low reliability between raters in several of the speech act codes. Codes S, J, N, and C show high variability. Visual inspection of these codes shows several disagreements: between the raters and errors. For these reasons, codes, S, J, N, and C were removed from the analysis.

Hotelling T2 Test:
To test our hypotheses, we use the Hotelling T2 test, which is a multivariate form of the univariate t-test (Hotelling, 1951). As with the t-test, this multivariate test assumes  H0  is true and samplingisfrom Np ( μ,Σ)andtestswhether H 0:  μ1 = μ 2or H 1:  μ1 ≠ μ 2. Thedistributionis determined by  p and the degrees of freedom,  v =  n1  + n 2 - 2, which is distributed as  T 2 p, n1+n2-2 when  H 0:   μ1  =  μ 2 is true. We reject  H 0 if  T2  >  T 2 α,  p ,  n1+n2-2 and otherwise accept  H 0 to be true. While the t-statistic compares the standardized difference between two observation means, the T 2 -statistic compares a standardized  distance between two observed sample mean  vectors.  If the distance is significant we become “suspicious” of the assumption that the mean vectors are equal and reject the null hypothesis,  H 0. 

Assumptions:
Several assumptions must be satisfied before using the Hotelling T2   test: independence, normality, and equality of covariance. We describe each below:
Independence:
First, the two groups must be independent of each other. In other words, the variables in each condition should not influence each other. We established independence by randomly assigning participants to condition and by ensuring that no participant repeated their participation in the experiment.
Normality:
Second, each population must follow the multivariate normal distribution. Shapiro-Wilk’s tests for each variable show several violations of the assumption of normality (see Appendix A). Since the sample size is relatively small this may affect the findings of significance, ie. p-values.
Equality of Covariance:
Third, the covariance matrices of the sample must be equal. Box’s M, χ 2   (15, N=33) = 37.08, p < .001. Consequently, we reject the null hypothesis--that the covariance matrices are equal--and assume that this assumption is violated. The accuracy of Box’s M test is very sensitive to departures from multivariate normality and unequal group sizes. Although there is a violation of the assumptions, we will proceed with conducting a Hotelling T2   test for the sake of this class project.
