<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $\Gamma=SL_2(\mathbb Z)$, $\mathbb H=\{\tau:\operatorname{Im}\tau>0\}$ and $q=e^{2\pi i\tau}$. The space $M_k$ consists of holomorphic functions on the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md) satisfying

$$
f\left(\frac{a\tau+b}{c\tau+d}\right)=(c\tau+d)^kf(\tau)\quad\left(\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\Gamma\right)
$$

and holomorphic at the cusp: their [Fourier expansion of a modular form](../../../../../../fourier-expansion-of-a-modular-form.md) is $f=\sum_{n\geq0}a_nq^n$. The subspace $S_k$ of [cusp forms](../../../../../../cusp-form.md) has $a_0=0$. Since all cusps are equivalent at level one, this condition treats every cusp. The element $-I$ forces odd-weight forms to vanish.

Use the permitted properties of the normalized [Eisenstein series](../../../../../../eisenstein-series.md) and [modular discriminant](../../../../../../modular-discriminant.md):

$$
E_4=1+240\sum_{n\geq1}\sigma_3(n)q^n,\qquad E_6=1-504\sum_{n\geq1}\sigma_5(n)q^n,\qquad \Delta=q\prod_{n\geq1}(1-q^n)^{24}.
$$

They have integer Fourier coefficients and weights $4,6,12$. For even $k\geq0$, the assumed dimension formula gives $d=\lfloor k/12\rfloor+1$ except when $k\equiv2\pmod{12}$, when $d=\lfloor k/12\rfloor$. For $0\leq j<d$, the remaining weight $k-12j$ is nonnegative and is not two. Choose $b_j\in\{0,1\}$ and $a_j\geq0$ with $4a_j+6b_j=k-12j$. Every allowable remaining weight admits such a choice. The forms

$$
F_j=\Delta^jE_4^{a_j}E_6^{b_j}=q^j+O(q^{j+1})
$$

give an [integral triangular basis of level-one modular forms](../../../../../../integral-triangular-basis-of-level-one-modular-forms.md): their distinct first exponents prove independence, and their number $d$ proves that they span.

Now take $f$ with integral coefficients. Subtract its constant coefficient times $F_0$. The remainder still has integral coefficients and has no constant term. Subtract its coefficient at $q$ times $F_1$, then its current coefficient at $q^2$ times $F_2$, and continue. Every subtraction uses an integer. After $d$ steps the remainder's first $d$ coefficients vanish; triangularity and the basis property force that remainder to be zero. Consequently

$$
\boxed{f=\sum_{j=0}^{d-1}b_j'\Delta^jE_4^{a_j}E_6^{b_j},\qquad b_j'\in\mathbb Z.}
$$

This proves integral polynomial generation without dividing by $1728$. The relation $E_4^3-E_6^2=1728\Delta$ explains why the additional integral generator is useful, although over $\mathbb C$ two generators suffice. For $k=0$ the basis is the constant one; when $M_k=0$, including weight two and odd weights, the claim is vacuous.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
