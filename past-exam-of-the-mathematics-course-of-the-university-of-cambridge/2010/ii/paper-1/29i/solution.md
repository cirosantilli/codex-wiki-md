<h1 id="29i/solution">Solution</h1>

↑ **Parent:** [29I](../29i.md)

A standard [Brownian motion](../../../../../brownian-motion-split.md) starts at zero, has continuous sample paths, independent stationary increments, and $W_t-W_s\sim\mathcal N(0,t-s)$ for $t>s$. The [Brownian reflection principle](../../../../../reflection-principle-wiener-process.md) reflects the increments after the first hitting time of a positive level and preserves Brownian law, by symmetry and the strong Markov property.

Reflect after the first hit of $x$. On the event that this hit occurs by time one, $W_1$ changes to $2x-W_1$. This is a measure-preserving involution taking the event $W_1\leq x-y$ to $W_1\geq x+y$, proving the specified identity for $x>0,y\geq0$; the $x=0$ case follows by symmetry. With $y=0$, the maximum event splits, up to zero-probability equality, into reflected equal halves. Thus

$$
\mathbb P(M\geq x)=2\mathbb P(W_1\geq x)=\mathbb P(|W_1|\geq x),\qquad x\geq0.
$$

Hence **$M$ and $|W_1|$ have the same distribution**, and $M>0$ almost surely.

For the ratio we need the joint law, not just these marginals. For $w<m$, the reflected identity gives $\mathbb P(M\geq m,W_1\leq w)=\mathbb P(W_1\geq2m-w)$. Differentiating yields

$$
f_{M,W_1}(m,w)=2(2m-w)\varphi(2m-w),\qquad m>0,\quad w<m,
$$

where $\varphi$ is the standard normal density. Put $w=rm$; the change of variables has Jacobian $m$. Therefore, for $r<1$,

$$
f_R(r)=\int_0^\infty2(2-r)m^2\varphi((2-r)m)\,dm
=\frac{2}{(2-r)^2}\int_0^\infty v^2\varphi(v)\,dv
=\boxed{\frac1{(2-r)^2}}.
$$

The density is zero for $r>1$ and has no atom at one. Its integral on $(-\infty,1)$ is one; negative ratios have no lower bound.

This gives the complete [Brownian terminal-to-maximum ratio](../../../../../brownian-terminal-to-maximum-ratio.md) law.

## ↑ Ancestors (10)

1. [29I](../29i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
