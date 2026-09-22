<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

Differentiating the [expectation value](../../../../../expectation-value.md) and using $\partial_t|\psi\rangle=-i\hat H|\psi\rangle/\hbar$ and $\partial_t\langle\psi|=i\langle\psi|\hat H/\hbar$ gives

$$
\boxed{\frac{d\langle\hat A\rangle}{dt}=\frac i\hbar\langle[\hat H,\hat A]\rangle+\left\langle\frac{\partial\hat A}{\partial t}\right\rangle.}
$$

The second term means explicit operator time dependence, distinct from the state's evolution.

The [commutator product rule](../../../../../commutator-product-rule.md) follows by adding and subtracting $\hat B\hat A\hat C$:

$$
[\hat A,\hat B\hat C]=\hat A\hat B\hat C-\hat B\hat C\hat A=[\hat A,\hat B]\hat C+\hat B[\hat A,\hat C].
$$

For the **[mathematical induction](../../../../../mathematical-induction.md) step**, let $\hat D=[\hat A,\hat B]$ and use $[\hat A,\hat D]=0$. The case $n=1$ is immediate. If $[\hat A^m,\hat B]=m\hat D\hat A^{m-1}$, then

$$
[\hat A^{m+1},\hat B]=\hat A^m\hat D+[\hat A^m,\hat B]\hat A=(m+1)\hat D\hat A^m.
$$

Thus the claimed identity holds for every positive integer. Commutation of $\hat B$ with $\hat D$ is not needed for this particular step. This is the [central-commutator differentiation rule](../../../../../central-commutator-differentiation-rule.md). Termwise application to a convergent [power series](../../../../../power-series.md), on a common domain where the operations are justified, gives

$$
\boxed{[F(\hat A),\hat B]=\sum_{n\geq1}na_n\hat D\hat A^{n-1}=\hat D F'(\hat A).}
$$

For [position](../../../../../position.md) and [momentum](../../../../../momentum-split.md), $[\hat x,\hat p]=i\hbar\hat I$. Hence $[\hat p^2,\hat x]=-2i\hbar\hat p$, $[V(\hat x),\hat x]=0$ and $[V(\hat x),\hat p]=i\hbar V'(\hat x)$. Substitution gives **[Ehrenfest theorem](../../../../../ehrenfest-theorem.md)**:

$$
\boxed{\frac{d\langle\hat x\rangle}{dt}=\frac{\langle\hat p\rangle}{m},\qquad\frac{d\langle\hat p\rangle}{dt}=-\langle V'(\hat x)\rangle.}
$$

The mean [momentum](../../../../../momentum-split.md) changes by the mean [force](../../../../../force-split.md). It does not follow for a general nonlinear [Potential energy](../../../../../potential-energy.md) that $\langle V'(\hat x)\rangle=V'(\langle\hat x\rangle)$: a closed classical trajectory for the mean [position](../../../../../position.md) requires an additional condition, such as a quadratic [Potential energy](../../../../../potential-energy.md) or a sufficiently localized [wave packet](../../../../../wave-packet.md).

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
