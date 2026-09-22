<h1 id="12g/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $|\lambda|<1$, let $F_\lambda(\zeta)=(\zeta-\lambda)/(1-\overline\lambda\zeta)$. Direct calculation gives

$$
1-|F_\lambda(\zeta)|^2=\frac{(1-|\lambda|^2)(1-|\zeta|^2)}{|1-\overline\lambda\zeta|^2}.
$$

Its denominator does not vanish in the disc, and this identity shows that it maps the disc into itself. Its inverse $(w+\lambda)/(1+\overline\lambda w)$ has the same property, so $F_\lambda$ is a [Poincare disc automorphism](../../../../../../poincare-disc-automorphism.md). Multiplication by a complex number of modulus one is another such automorphism.

Conversely let $T$ be a [Möbius transformation](../../../../../../mobius-transformation.md) mapping the disc onto itself, and let $\lambda=T^{-1}(0)$. Then $T\circ F_\lambda^{-1}$ is a disc automorphism fixing zero, say $S(\zeta)=a\zeta/(c\zeta+d)$ with $d\ne0$. Since it maps the boundary circle to itself, $|a|^2=|c\zeta+d|^2=|c|^2+|d|^2+2\operatorname{Re}(c\overline d\zeta)$ for every $|\zeta|=1$. This forces $c\overline d=0$, hence $c=0$ and $|a/d|=1$. Thus $S$ is a rotation $\eta\zeta$, and $T=\eta F_\lambda$. Absorb the denominator's minus sign into $\omega=-\eta$ to obtain precisely the paper's convention:

$$
\boxed{T(\zeta)=\omega\frac{\zeta-\lambda}{\overline\lambda\zeta-1},\qquad |\lambda|<1,\quad|\omega|=1.}
$$

Here mapping the disc to itself means bijectively onto itself; there are nonautomorphic [Möbius transformations](../../../../../../mobius-transformation.md) whose image is a proper subdisc.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [12G](../../12g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
