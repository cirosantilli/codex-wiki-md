<h1 id="13a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply the Hankel representation with $z$ replaced by $1-z$:

$$
\zeta(1-z)=\frac{\Gamma(z)}{2\pi i}
\int_H\frac{t^{-z}}{e^{-t}-1}\,dt.
$$

Enlarge $H$ to a modified Hankel contour that encloses the simple poles $t=2\pi i n$, $n\in\mathbb Z\setminus\{0\}$. In a strip where the deformation and residue sum converge, the outer pieces vanish and the orientation gives the Hankel integral as minus $2\pi i$ times the sum of the enclosed residues. Part (b) gives

$$
\begin{aligned}
\sum_{n\ne0}\operatorname{Res}_{t=2\pi i n}
\frac{t^{-z}}{e^{-t}-1}
&=-\sum_{n=1}^{\infty}\left[(2\pi i n)^{-z}+(-2\pi i n)^{-z}\right]\\
&=-2(2\pi)^{-z}\cos\!\left(\frac{\pi z}{2}\right)\zeta(z).
\end{aligned}
$$

Substitution therefore yields

$$
\boxed{\zeta(1-z)=2^{1-z}\pi^{-z}
\cos\!\left(\frac{\pi z}{2}\right)\Gamma(z)\zeta(z).}
$$

Both sides are meromorphic functions of $z$, so the [identity theorem](../../../../../../identity-theorem.md) extends the equality from the initial strip to every point where either side is defined.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [13A](../../13a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
