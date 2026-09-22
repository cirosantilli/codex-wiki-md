<h1 id="14b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Neglect the decaying mode from part a. A mode that enters during matter domination grows in amplitude by

$$
\frac{a(t_0)}{a(t_H)}
=\left(\frac{t_0}{t_H}\right)^{2/3},
$$

so its variance grows by $(t_0/t_H)^{4/3}$. For $k<k_{\rm eq}$, part b gives

$$
P(k)=\frac{C}{k^3}
\left(\frac{k}{k_0}\right)^4
=\boxed{\frac{Ck}{k_0^4}}.
$$

For $k>k_{\rm eq}$, the mode enters during radiation domination and is assumed not to grow significantly until equality. It then grows by $a(t_0)/a_{\rm eq}$. Since the equality mode satisfies

$$
\frac{t_{\rm eq}}{t_0}
=\left(\frac{k_0}{k_{\rm eq}}\right)^3,
$$

the post-equality variance growth is

$$
\left(\frac{a(t_0)}{a_{\rm eq}}\right)^2
=\left(\frac{t_0}{t_{\rm eq}}\right)^{4/3}
=\left(\frac{k_{\rm eq}}{k_0}\right)^4.
$$

Therefore the [broken matter power spectrum from horizon entry](../../../../../../broken-matter-power-spectrum-from-horizon-entry.md) is

$$
\boxed{
P(k)=V\langle|\delta_k(t_0)|^2\rangle
=
\begin{cases}
\dfrac{Ck}{k_0^4},&k<k_{\rm eq},\\[6pt]
\dfrac{Ck_{\rm eq}^4}{k^3k_0^4},&k>k_{\rm eq}.
\end{cases}}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [14B](../../14b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
