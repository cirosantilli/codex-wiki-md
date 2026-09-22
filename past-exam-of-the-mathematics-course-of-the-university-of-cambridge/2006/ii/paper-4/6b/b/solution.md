<h1 id="6b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [similarity solution](../../../../../../similarity-solution.md), differentiation gives

$$
n_t=-\mu n-\frac{e^{-\mu t}\dot\lambda}{\lambda^2}(f+\eta f'),\qquad
(nn_x)_x=\frac{e^{-2\mu t}}{\lambda^4}(ff')'.
$$

Choose $\lambda^2\dot\lambda=e^{-\mu t}$. The remaining equation is $-(\eta f)'=(ff')'$. Its integration constant is zero for the required decaying or compactly supported profile, so $f(f'+\eta)=0$. Where $f>0$, this gives $f'=-\eta$. For a nonnegative population the complete profile is therefore

$$
f(\eta)=\frac12(b^2-\eta^2)_+.
$$

Normalization gives $Q=2b^3/3$, hence $b=(3Q/2)^{1/3}$. Integrating the scale equation with zero initial scale yields

$$
\lambda(t)^3=\frac3\mu(1-e^{-\mu t}).
$$

Thus

$$
\boxed{n(x,t)=\frac{e^{-\mu t}}{2\lambda(t)}
\left[b^2-\frac{x^2}{\lambda(t)^2}\right]_+,\quad
b=(3Q/2)^{1/3},\quad \lambda(t)=\left[\frac3\mu(1-e^{-\mu t})\right]^{1/3}}.
$$

Its support satisfies

$$
\boxed{|x|\le b\lambda(t)=\left[\frac{9Q}{2\mu}(1-e^{-\mu t})\right]^{1/3}
\le\left(\frac{9Q}{2\mu}\right)^{1/3}}.
$$

The profile is a [weak solution](../../../../../../weak-solution.md) at its moving edges, where $nn_x$ vanishes. As $t\downarrow0$ its support shrinks to the origin and its mass tends to $Q$, so its initial distribution is $Q\delta_0$. The bounded limiting range assumes $\mu>0$; at zero death rate the scale instead grows as $(3t)^{1/3}$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6B](../../6b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
