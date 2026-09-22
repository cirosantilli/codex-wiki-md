<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The specified Bell-state [phases](../../../../../phase-waves.md) give

$$
a_1=\frac{b_2+ib_3}{\sqrt2},\quad
a_4=\frac{b_2-ib_3}{\sqrt2},\quad
a_2=\frac{ib_1+b_4}{\sqrt2},\quad
a_3=\frac{ib_1-b_4}{\sqrt2}.
$$

Therefore

$$
a_1a_4-a_2a_3
=\frac12(b_2^2+b_3^2+b_1^2+b_4^2),
\qquad
\boxed{\det\rho_A=\frac14\left|\sum_{j=1}^4b_j^2\right|^2.}
$$

The sum contains complex squares, not squared moduli. Define $q=\sum_jb_j^2$ and $\mathcal C=|q|$. Normalization gives $\sum_j|b_j|^2=1$, so the [triangle inequality](../../../../../triangle-inequality.md) ensures $0\leq\mathcal C\leq1$.

The [characteristic polynomial](../../../../../characteristic-polynomial.md) is $\lambda^2-\lambda+\mathcal C^2/4$. Hence

$$
\boxed{\lambda_\pm=\frac12\left(1\pm\sqrt{1-\mathcal C^2}\right),\qquad
S_A=-\lambda_+\ln\lambda_+-\lambda_-\ln\lambda_-.}
$$

Here logarithms are natural and $0\ln0$ means its limiting value zero. Using logarithms to base two gives entropy in bits instead. [Product states](../../../../../product-state.md) have $\mathcal C=0$, [spectrum](../../../../../spectrum-functional-analysis.md) $(1,0)$ and entropy zero; [maximally entangled states](../../../../../maximally-entangled-state.md) have $\mathcal C=1$, [spectrum](../../../../../spectrum-functional-analysis.md) $(1/2,1/2)$ and entropy $\ln2$.

This phased [Bell basis](../../../../../bell-basis.md) is a [magic basis](../../../../../magic-basis.md), and $\mathcal C$ is the pure-state [concurrence](../../../../../concurrence.md). The paper's ordering is a permutation of the usual magic-basis ordering, which leaves $|\sum_jb_j^2|$ unchanged.[Eqs.(3)–(6), magic basis, concurrence and binary entropy](../../../../../entanglement-of-a-pair-of-quantum-bits-by-scott-hill-and-william-k-wootters.md)

<a id="2/b/image-original-two-qubit-calculation-of-the-reduced-eigenvalues-and-entropy-as-functions-of-concurrence"></a>
![](../../../../../past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge/2016/paper-1-concurrence-entropy.png)

**[Figure 2](#2/b/image-original-two-qubit-calculation-of-the-reduced-eigenvalues-and-entropy-as-functions-of-concurrence). Original two-qubit calculation of the reduced eigenvalues and entropy as functions of concurrence**.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
