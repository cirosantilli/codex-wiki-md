<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $w=2k$. For a positive-determinant real [matrix](../../../../../../matrix.md) $A=\begin{pmatrix}a&b\\c&d\end{pmatrix}$, extend the [slash operator for modular forms](../../../../../../slash-operator-for-modular-forms.md) by

$$
(f|_wA)(\tau)=(\det A)^{w/2}(c\tau+d)^{-w}f(A\tau).
$$

Let $\mathcal M_n$ be the integral [matrices](../../../../../../matrix.md) of [determinant](../../../../../../determinant.md) $n>0$. Each left $SL_2(\mathbb Z)$ [orbit](../../../../../../orbit-dynamical-system.md) has a unique representative $\begin{pmatrix}a&b\\0&d\end{pmatrix}$ with $ad=n$, $a,d>0$, $0\leq b<d$. To obtain it, the [Euclidean algorithm](../../../../../../euclidean-algorithm.md) on the first column produces $(a,0)$ with $a>0$; the [determinant](../../../../../../determinant.md) fixes $d$, and a row shear reduces $b$ modulo $d$. This also proves uniqueness.

Define the normalized [Hecke operator](../../../../../../hecke-operator.md)

$$
\boxed{T_w(n)f=n^{w/2-1}\sum_{A\in SL_2(\mathbb Z)\backslash\mathcal M_n}f|_wA
=n^{w-1}\sum_{ad=n}d^{-w}\sum_{b=0}^{d-1}f\left(\frac{a\tau+b}{d}\right).}
$$

Right multiplication by $SL_2(\mathbb Z)$ permutes these left orbits, and the slash operation is associative. Hence the sum satisfies the same [modular form](../../../../../../modular-form.md) transformation law. It is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) on $\mathbb H$ since each argument stays there.

For $f=\sum_{r\geq0}c(r)q^r$, summing the phase $e^{2\pi irb/d}$ over $b$ gives zero unless $d\mid r$, and gives $d$ when $d\mid r$. For the resulting term to contribute to $q^m$, one needs $a\mid m$ and $r=dm/a=nm/a^2$. Its scalar factor is $n^{w-1}d^{1-w}=a^{w-1}$. Thus

$$
\boxed{T_w(n)f=\sum_{m\geq0}\left(\sum_{a\mid\gcd(n,m)}a^{w-1}c\left(\frac{nm}{a^2}\right)\right)q^m,}
$$

where $\gcd(n,0)=n$. All powers are nonnegative, so the sum is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) at infinity and belongs to $M_w$; level one has only this [modular cusp](../../../../../../cusp-of-a-modular-group.md) class. Its constant coefficient is $\sigma_{w-1}(n)c(0)$, so [modular cusp](../../../../../../cusp-of-a-modular-group.md) forms are preserved. This is the full [Fourier coefficients of a composite-index Hecke operator](../../../../../../fourier-coefficients-of-a-composite-index-hecke-operator.md) formula, including the constant term.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
