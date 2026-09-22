<h1 id="1/1/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $\Phi_t,\Psi_s$ be the [local flows](../../../../../../../local-flow.md) of $X,Y$. The derivative of the pullback of $Y$ by $\Phi_t$ is $\Phi_t^*[X,Y]$. Therefore $[X,Y]=0$ makes $Y$ invariant under the $X$ flow. For fixed $t$, the two curves $\Phi_t(\Psi_s(p))$ and $\Psi_s(\Phi_t(p))$ then solve the same initial-value problem for $Y$. Uniqueness gives commuting flows wherever both compositions are defined. Conversely, commutation implies invariance of $Y$ under $\Phi_t$, and differentiation at $t=0$ gives $\boxed{[X,Y]=0}$. This proves [vanishing Lie bracket is equivalent to commuting local flows](../../../../../../../vanishing-lie-bracket-is-equivalent-to-commuting-local-flows.md).

For the contraction $\eta$, commute each [Lie derivative](../../../../../../../lie-derivative-of-a-differential-form.md) past the other interior products using $[\mathcal L_{X_i},\iota_{X_j}]=\iota_{[X_i,X_j]}=0$. Each $\mathcal L_{X_i}\omega$ is zero by volume preservation. [Cartan's magic formula](../../../../../../../cartan-s-magic-formula.md) $d\iota_X=\mathcal L_X-\iota_Xd$, applied successively, now gives

$$
d\eta=\sum_{i=1}^n(-1)^{i-1}\iota_{X_1}\cdots\widehat{\iota_{X_i}}\cdots\iota_{X_n}\mathcal L_{X_i}\omega
+(-1)^n\iota_{X_1}\cdots\iota_{X_n}d\omega=0.
$$

The last term vanishes since $\omega$ has top degree. Hence $\boxed{\eta\text{ is closed}}$.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 115](../../../../paper-115-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
