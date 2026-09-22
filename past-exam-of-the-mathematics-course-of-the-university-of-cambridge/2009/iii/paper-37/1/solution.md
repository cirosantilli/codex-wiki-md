<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $m_j=\mathbb EY^j$ and $M=M_Y$. The derivatives of the [cumulant-generating function](../../../../../cumulant-generating-function.md) are

$$
\kappa_Y'=\frac{M'}M,\qquad \kappa_Y''=\frac{M''}M-\frac{(M')^2}{M^2},\qquad \kappa_Y'''=\frac{M'''}M-\frac{3M'M''}{M^2}+\frac{2(M')^3}{M^3}.
$$

Since $M(0)=1$ and $M^{(j)}(0)=m_j$, the first three [cumulants](../../../../../cumulant.md) are

$$
\boxed{\kappa_{Y,1}=m_1=\mathbb EY,\quad \kappa_{Y,2}=m_2-m_1^2=\operatorname{Var}(Y),\quad \kappa_{Y,3}=m_3-3m_1m_2+2m_1^3=\mathbb E(Y-\mathbb EY)^3.}
$$

The last equality follows by expanding the cube and taking [expectations](../../../../../expected-value.md). We use the paper's unstandardized third [central moment](../../../../../central-moment.md) throughout. The usual [skewness](../../../../../skewness.md) coefficient divides this quantity by $\operatorname{Var}(Y)^{3/2}$; its sign is the same whenever the [variance](../../../../../variance-split.md) is positive.

There is a minor domain qualification: finite ordinary [moments](../../../../../moment.md) do not guarantee a finite [moment-generating function](../../../../../moment-generating-function.md) for positive arguments. The differentiations are valid in a neighborhood of zero when a positive exponential moment exists. For positive variables with the stated finite [moments](../../../../../moment.md), all formulas also follow from left derivatives at zero, because $Y^j e^{tY}\le Y^j$ for $t\le0$ and [dominated convergence](../../../../../dominated-convergence-theorem.md) applies. Thus no extra exponential-moment assumption is needed for the moment identities themselves.

For the [random sum of independent claims](../../../../../random-sum-of-independent-claims.md), condition on $N=k$. Independence of the claims and independence from the count give

$$
\mathbb E[e^{tS}\mid N=k]=M_{X_1}(t)^k.
$$

Taking [expectations](../../../../../expected-value.md) and then logarithms yields the [random-sum transform identity](../../../../../random-sum-transform-identity.md) and the [cumulant composition for a random sum](../../../../../cumulant-composition-for-a-random-sum.md):

$$
\boxed{M_S(t)=G_N(M_{X_1}(t)),\qquad\kappa_S(t)=\kappa_N(\log M_{X_1}(t))=\kappa_N(\kappa_{X_1}(t)).}
$$

Here $G_N$ is the [probability generating function](../../../../../probability-generating-function.md). These identities hold wherever the transforms are finite, in particular for $t\le0$ with positive claims.

For reuse in the three cases, write $m_j=\mathbb EX_1^j$ and $a_j=\kappa_{N,j}$. Applying the chain rule three times gives

$$
\kappa_{S,3}=a_1(m_3-3m_1m_2+2m_1^3)+3a_2m_1(m_2-m_1^2)+a_3m_1^3,
$$

or equivalently

$$
\kappa_{S,3}=a_1m_3+3(a_2-a_1)m_1m_2+(a_3-3a_2+2a_1)m_1^3.
$$

This expresses the requested third [central moment](../../../../../central-moment.md) in raw claim [moments](../../../../../moment.md), while keeping the contribution of claim-count variability explicit.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
