<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [geometrized units](../../../../../../../geometrized-units.md) $G=c=1$. For a stationary [asymptotically flat spacetime](../../../../../../../asymptotically-flat-spacetime.md), normalize the timelike [Killing vector field](../../../../../../../killing-vector-field.md) $\xi$ to have squared norm $-1$ at infinity. The [Komar mass](../../../../../../../komar-mass.md) is

$$
M_K=-\frac1{8\pi}\lim_{S\to\infty}\int_S\nabla^a\xi^b\,dS_{ab}.
$$

Here the oriented binormal is chosen so that an ordinary positive-mass static solution gives a positive integral. Equivalently, on a static slice with lapse $N=\sqrt{-\xi^2}$ and outward spatial unit normal $s^i$,

$$
M_K=\frac1{4\pi}\lim_{S\to\infty}\int_Ss^iD_iN\,dA.
$$

This second expression fixes the orientation unambiguously and is convenient for the [Majumdar–Papapetrou solution](../../../../../../../majumdar-papapetrou-solution.md).

The spatial metric is $\gamma_{ij}=H^2\delta_{ij}$ and $N=H^{-1}$. On a large coordinate sphere, $s^i=H^{-1}\widehat r^i$ and $dA=H^2r^2d\Omega$. Thus

$$
s^iD_iN\,dA=-\frac{r^2}{H}\partial_rH\,d\Omega,\qquad M_K=-\frac1{4\pi}\lim_{r\to\infty}\int_{S^2}\frac{r^2\partial_rH}{H}\,d\Omega.
$$

The original PDF has the [Euclidean norm](../../../../../../../euclidean-norm.md) in each source denominator, which is missing in the TeX aid. With that norm, the [harmonic function](../../../../../../../harmonic-function.md) has asymptotics

$$
H=1+\frac{\sum_iM_i}{r}+O(r^{-2}),\qquad\partial_rH=-\frac{\sum_iM_i}{r^2}+O(r^{-3}).
$$

Therefore

$$
\boxed{M_K=\sum_{i=1}^NM_i.}
$$

If $M_i$ are retained as length parameters while $G$ is restored, the physical mass is $\sum_iM_i/G$. This is the charge at infinity. A [Komar integral](../../../../../../../komar-charge.md) is not generally surface-independent here, since [Einstein-Maxwell theory](../../../../../../../einstein-maxwell-theory.md) has the electromagnetic [stress-energy tensor](../../../../../../../stress-energy-tensor.md) between the surfaces; in particular it should not be confused with a sum of vacuum horizon [Komar charges](../../../../../../../komar-charge.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 66](../../../../paper-66-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
