<h1 id="34c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Maximize the [Gibbs entropy](../../../../../../gibbs-entropy.md) subject to normalization and the two mean constraints. Introduce multipliers $\eta,A,B$ and differentiate

$$
-k\sum_i\rho_i\log\rho_i-\eta(\sum_i\rho_i-1)
-A(\sum_i\rho_iE_i-E)-B(\sum_i\rho_iN_i-N).
$$

Stationarity gives $\rho_i\propto\exp[-(AE_i+BN_i)/k]$. Strict concavity of entropy gives the constrained maximum, on its support. Differentiating the maximum value with respect to the constrained means, or differentiating the entropy along the maximizing distribution and using $\sum_i d\rho_i=0$, gives $dS=A\,dE+B\,dN$. The thermodynamic identification is $A=1/T$, $B=-\mu/T$. Therefore

$$
\boxed{\frac{\partial S}{\partial E}=\frac1T,\qquad
\frac{\partial S}{\partial N}=-\frac\mu T,\qquad
\overline\rho_i=\mathcal Z^{-1}e^{-(E_i-\mu N_i)/(kT)}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [34C](../../34c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
