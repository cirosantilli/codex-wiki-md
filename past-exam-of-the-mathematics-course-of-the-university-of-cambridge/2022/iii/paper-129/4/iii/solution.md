<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $M(a)=\max_{\gamma\in\widehat G}|\widehat{\partial_af}(\gamma)|^2$. By the [Derivative identity for the Gowers U3 norm](../../../../../../derivative-identity-for-the-gowers-u3-norm.md), the Fourier formula for the $U^2$ norm, and [Parseval identity](../../../../../../parseval-identity.md),

$$
c\leq\mathbb E_a\sum_\gamma|\widehat{\partial_af}(\gamma)|^4
\leq\mathbb E_a M(a)\sum_\gamma|\widehat{\partial_af}(\gamma)|^2
\leq\mathbb E_aM(a),
$$

because $\|f\|_\infty\leq1$. Let

$$
B=\{a:M(a)\geq c/2\},
$$

and for every $a\in B$ choose $\phi(a)\in\widehat G$ attaining $M(a)$. Then

$$
|\widehat{\partial_af}(\phi(a))|^2\geq c/2
$$

for every $a\in B$, and deleting the complement of $B$ from the preceding average leaves total mass at least $c/2$.

Let $\Gamma_\phi=\{(a,\phi(a)):a\in B\}\subseteq G\times\widehat G$. The box-norm inequality applied to the selected Fourier coefficients and the cocycle identity for multiplicative derivatives gives

$$
\left(\mathbb E_a1_B(a)|\widehat{\partial_af}(\phi(a))|^2\right)^8
\leq\frac{E(\Gamma_\phi)}{|G|^3}.
$$

The left side is at least $(c/2)^8$. An additive quadruple in $\Gamma_\phi$ is exactly a tuple $(a,b,c,d)\in B^4$ satisfying

$$
a+b=c+d,
\qquad
\phi(a)\phi(b)=\phi(c)\phi(d).
$$

**Therefore there are at least $(c/2)^8|G|^3$ such quadruples, which is the [Frequency graph extracted from a large Gowers U3 norm](../../../../../../frequency-graph-extracted-from-a-large-gowers-u3-norm.md).**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
