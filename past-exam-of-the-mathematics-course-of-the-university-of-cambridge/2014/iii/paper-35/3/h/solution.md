<h1 id="3/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

Put $\kappa_i=n/(n+q_i)$. The [posterior mean](../../../../../../posterior-mean.md) of the [Gaussian practical-null mixture](../../../../../../gaussian-practical-null-mixture.md) is

$$
\mathbb E[\beta\mid y]=[w_0(y)\kappa_0+w_1(y)\kappa_1]y.
$$

Near zero, $B_{01}(0)>1$, so the narrow component has high [posterior probability](../../../../../../posterior-probability.md) and $\kappa_0$ is small when $n_0\gg n$. This pulls the [Bayesian model averaging](../../../../../../bayesian-model-averaging.md) posterior toward zero. For the given ratios, writing $z=\sqrt n\,y$ gives

$$
B_{01}(y)=10e^{-99z^2/202},\qquad B_{01}>1\ \Longleftrightarrow\ |z|<2.16753\ldots.
$$

Thus the order statement $y=O(n^{-1/2})$ alone does not guarantee strong pull toward zero: $z=3$ already has the opposite model preference.

As $|y|$ grows, $V_1>V_0$ makes $B_{01}(y)\to0$, and the [mixture model](../../../../../../mixture-model.md) approaches $N(\kappa_1 y,1/(n+q_1))$. **Its center is exactly $\kappa_1 y$, and approximately $y$ only for a sufficiently diffuse wide prior**, meaning $q_1\ll n$. Here $\kappa_1=100/101$, so the relative displacement is about one percent. Large observations alone do not remove this finite-prior shrinkage.

## ↑ Ancestors (11)

1. [H](../h.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
