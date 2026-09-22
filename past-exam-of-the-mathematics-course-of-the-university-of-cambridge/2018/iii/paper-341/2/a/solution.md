<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The nodes $0,1/2,1$ have [Lagrange interpolation polynomials](../../../../../../lagrange-polynomial.md)

$$
\ell_1(s)=2s^2-3s+1,\quad
\ell_2(s)=4s-4s^2,\quad
\ell_3(s)=2s^2-s.
$$

The coefficients obtained from $a_{ij}=\int_0^{c_i}\ell_j(s)\,ds$ and $b_j=\int_0^1\ell_j(s)\,ds$ reproduce the given [Butcher tableau](../../../../../../butcher-tableau.md). In particular, the second row's last entry is $-1/24$, which is missing from the TeX transcription. Thus this is the three-stage [Lobatto IIIA method](../../../../../../lobatto-iiia-method.md).

One applicable collocation theorem is that $s$-stage Lobatto IIIA collocation has order $2s-2$. Alternatively, the [fourth-order conditions for a Runge-Kutta method](../../../../../../fourth-order-conditions-for-a-runge-kutta-method.md) give a direct verification. With $e=(1,1,1)^T$, $c=Ae$ and $C=\operatorname{diag}(c)$, the eight required [Butcher order conditions](../../../../../../butcher-order-condition.md) are

$$
\begin{gathered}
b^Te=1,\quad b^Tc=\tfrac12,\quad b^Tc^2=\tfrac13,\quad b^TAc=\tfrac16,\\
b^Tc^3=\tfrac14,\quad b^TCAc=\tfrac18,\quad
b^TAc^2=\tfrac1{12},\quad b^TA^2c=\tfrac1{24}.
\end{gathered}
$$

Powers of $c$ here are componentwise. Substitution satisfies all eight. The [stability function](../../../../../../stability-function.md) computed from the stages is

$$
R(z)=1+zb^T(I-zA)^{-1}e
=\frac{1+z/2+z^2/12}{1-z/2+z^2/12}.
$$

Its expansion satisfies $R(z)-e^z=-z^5/720+O(z^6)$, so even the scalar linear problem fails the fifth-order condition. Hence

$$
\boxed{p=4.}
$$

The [Butcher order condition](../../../../../../butcher-order-condition.md) theorem equates order $p$ with all conditions for [rooted trees](../../../../../../rooted-tree.md) through order $p$; the displayed conditions are its complete specialization through order four.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
