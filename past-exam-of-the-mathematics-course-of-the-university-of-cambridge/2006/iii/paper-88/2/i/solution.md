<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [Hecke-normalized rational slash operator](../../../../../../hecke-normalized-rational-slash-operator.md) from the PDF, writing $f[\alpha]_k$ for its right action. Put $A_D=\operatorname{diag}(D,1)$. If $\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\Gamma_0(N)$, then

$$
A_D\gamma A_D^{-1}=\begin{pmatrix}a&Db\\c/D&d\end{pmatrix}\in\Gamma_0(M).
$$

Indeed $N/D$ is an integer divisible by $M$, so $c/D$ is an integer divisible by $M$. The ordinary weight transformation of the original [cusp form](../../../../../../cusp-form.md) therefore gives

$$
f(D\gamma\tau)=(c\tau+d)^k f(D\tau).
$$

Thus $g(\tau)=f(D\tau)$ has the correct transformation for the [Gamma 0 congruence subgroup](../../../../../../gamma-0-congruence-subgroup.md) at level $N$, and it is holomorphic in the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md).

It remains to check every [modular cusp](../../../../../../cusp-of-a-modular-group.md), not just infinity. Let $\rho\in SL_2(\mathbb Z)$ carry infinity to that cusp, and choose $\sigma\in SL_2(\mathbb Z)$ with $\sigma\infty=A_D\rho\infty$. The matrix $B=\sigma^{-1}A_D\rho$ is upper triangular over the rationals, with positive ratio of diagonal entries. Therefore, up to a nonzero constant weight factor,

$$
g[\rho]_k=(f[\sigma]_k)[B]_k.
$$

The original cusp expansion of $f[\sigma]_k$ has only positive exponents. The change $\tau\mapsto r\tau+s$ induced by $B$, with $r>0$, preserves exponential decay as $\operatorname{Im}\tau\to\infty$. The transformed function also has a positive integral period because $g$ is modular for a finite-index subgroup. Its bounded periodic holomorphic expansion consequently has no negative exponents and its limiting constant term is zero. This proves [cusp holomorphy under rational slash operators](../../../../../../cusp-holomorphy-under-rational-slash-operators.md) and establishes the [degeneracy map for cusp forms](../../../../../../degeneracy-map-for-cusp-forms.md):

$$
\boxed{f(D\tau)\in S_k(\Gamma_0(N)).}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 88](../../../paper-88-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
