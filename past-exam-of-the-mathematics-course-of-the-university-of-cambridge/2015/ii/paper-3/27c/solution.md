<h1 id="27c/solution">Solution</h1>

↑ **Parent:** [27C](../27c.md)

Use the entire function $e^{ikz^3}$. The [steepest descent contour](../../../../../steepest-descent-contour.md) starting at $1$ is

$$
\boxed{z(u)=(1+iu)^{1/3},\quad0\leq u<\infty,}
$$

with the cube-root branch starting at $1$. Along it $ikz^3=ik-ku$, so the real part decreases and the imaginary part stays constant. It approaches the ray $\arg z=\pi/6$, on which $z=e^{i\pi/6}u^{1/3}$ and $ikz^3=-ku$.

Close a contour using the interval $[0,1]$, these two outgoing paths truncated at parameter $R$, and a short connecting arc. The two endpoints differ by $O(R^{-2/3})$, and the integrand on the connector decays exponentially in $R$. [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md) therefore gives $\int_0^1e^{ikt^3}\,dt=I_1-I_2$.

The specified substitutions give

$$
I_1=\frac{e^{i\pi/6}}3\int_0^\infty e^{-ku}u^{-2/3}\,du=\frac{e^{i\pi/6}\Gamma(1/3)}{3k^{1/3}},
$$

and

$$
I_2=\frac{ie^{ik}}3\int_0^\infty e^{-ku}(1+iu)^{-2/3}\,du.
$$

Expand $(1+iu)^{-2/3}=1-2iu/3+O(u^2)$ near zero, and apply [Watson lemma](../../../../../watson-s-lemma.md), or split the integral at a fixed small $u$ and integrate the Taylor remainder. This gives **the first two asymptotic terms**

$$
\boxed{\int_0^1e^{ikt^3}\,dt=\frac{e^{i\pi/6}\Gamma(1/3)}{3k^{1/3}}-\frac{ie^{ik}}{3k}+O(k^{-2}).}
$$

Keeping the next term gives $-2e^{ik}/(9k^2)+O(k^{-3})$. The fractional power comes from the degenerate stationary endpoint at zero; the oscillatory integer-power terms come from the ordinary endpoint at one.

## ↑ Ancestors (10)

1. [27C](../27c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
