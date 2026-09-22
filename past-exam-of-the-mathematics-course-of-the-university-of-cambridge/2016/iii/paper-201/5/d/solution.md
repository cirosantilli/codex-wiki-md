<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Fix $x\in(-1,1)$ and start at $(x,y)$ with $y>1$. Write the independent Brownian coordinates as $x+W_t^1$ and $y+W_t^2$. Let

$$
H=\inf\{t:|x+W_t^1|=1\},
\qquad L_y=\inf\{t:y+W_t^2=1\}.
$$

On $\{H<L_y\}$ the path has stayed in the upper strip and first exits the cross-shaped domain at its right or left side. The boundary value is $a$ or $b$, respectively. Let $V=a$ if $x+W_H^1=1$ and $V=b$ if $x+W_H^1=-1$. The [Brownian exit from an interval](../../../../../../brownian-exit-from-an-interval.md) probabilities give

$$
\mathbb E V=a\frac{1+x}{2}+b\frac{1-x}{2}
=\frac{a+b}{2}+\frac{a-b}{2}x.
$$

Couple all heights $y$ using the same two Brownian paths. By part (a), $H<\infty$ almost surely, and continuity makes $\min_{0\leq t\leq H}W_t^2$ finite. Thus

$$
\mathbb P(L_y\leq H)
=\mathbb P\left(\min_{0\leq t\leq H}W_t^2\leq1-y\right)\longrightarrow0.
$$

Let $K=\max\{|a|,|b|,|c|,|d|\}$. On the complement of this exceptional event, $f(B_T)=V$; on the event itself, $|f(B_T)-V|\leq2K$. The representation in part (c) therefore yields

$$
\left|u(x,y)-\mathbb E V\right|\leq2K\,\mathbb P(L_y\leq H)\longrightarrow0.
$$

This proves the [harmonic limit along an infinite strip arm](../../../../../../harmonic-limit-along-an-infinite-strip-arm.md):

$$
\boxed{\lim_{y\to\infty}u(x,y)=\frac{a+b}{2}+\frac{a-b}{2}x.}
$$

**Far up the arm, the bottom is reached with vanishing probability before the horizontal coordinate exits.** The limit is consequently determined by the two side values alone.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
