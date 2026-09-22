<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the constant-$H$ [de Sitter approximation](../../../../../../de-sitter-approximation.md), $a=-1/(H\tau)$ with $\tau<0$, so $a''/a=2/\tau^2$. The massive rescaled mode obeys

$$
v_{\mathbf k}''+\left[k^2+\frac{m_\chi^2/H^2-2}{\tau^2}\right]v_{\mathbf k}=0.
$$

For a fixed mass in the specified open interval, at sufficiently late [superhorizon scales](../../../../../../superhorizon-scale.md) with $|k\tau|\ll1$, the $k^2$ term is negligible compared with the inverse-square term in the limiting equation. Try $v\propto(-\tau)^p$. The indicial equation is $p(p-1)+m_\chi^2/H^2-2=0$, giving

$$
\boxed{p=\frac12\pm\nu,\qquad
\nu=\sqrt{\frac94-\frac{m_\chi^2}{H^2}}.}
$$

Thus both independent branches of the [massive de Sitter superhorizon scalar mode](../../../../../../massive-de-sitter-superhorizon-scalar-mode.md) are present in

$$
\boxed{v_{\mathbf k}=\frac1{\sqrt{2k}}\left[
c_-(k)(-k\tau)^{1/2-\nu}+c_+(k)(-k\tau)^{1/2+\nu}\right].}
$$

The coefficients are constant in time and fixed by initial conditions. Writing $-k\tau>0$ avoids ambiguous fractional powers of the negative number $k\tau$; a chosen complex phase in the printed notation can be absorbed into the coefficients.

For the specified mass range, $1/2<\nu<\sqrt5/2<3/2$. The physical fluctuation is $\delta\chi_{\mathbf k}=v_{\mathbf k}/a=-H\tau v_{\mathbf k}$, so its two branches behave as $(-\tau)^{3/2-\nu}$ and $(-\tau)^{3/2+\nu}$. Both exponents are strictly positive. Therefore **both physical-field branches decay as $\tau\to0^-$**:

$$
\boxed{\delta\chi_{\mathbf k}\propto
\begin{cases}a^{-(3/2-\nu)},&\text{slower branch},\\
a^{-(3/2+\nu)},&\text{faster branch}.
\end{cases}}
$$

The slower branch of $v$ itself grows because $1/2-\nu<0$, but the expanding [scale factor](../../../../../../scale-factor-cosmology.md) more than cancels that growth. A spatially homogeneous background field of this mass satisfies the corresponding $k=0$ equation and also has these decaying powers.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 310](../../../paper-310-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
