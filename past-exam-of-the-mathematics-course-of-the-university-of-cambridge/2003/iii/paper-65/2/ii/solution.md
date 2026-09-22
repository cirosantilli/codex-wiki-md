<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take $A>0$ and a nontrivial nonnegative profile. On $0<r<R(t)$ put $X=(R/r)^a$ and $\Sigma=\sigma(X-1)$. The diffusion operator acts on $r^{1/2}\bar\nu\Sigma=A\sigma^2[r^{5/2-2a}R^{2a}-2r^{5/2-a}R^a+r^{5/2}]$, giving

$$
\partial_t\Sigma=3A\sigma^2\left[(\tfrac52-2a)(2-2a)X^2-2(\tfrac52-a)(2-a)X+5\right].
$$

But differentiating the trial profile in time gives only

$$
\partial_t\Sigma=\left(\dot\sigma+a\sigma\frac{\dot R}{R}\right)X-\dot\sigma.
$$

For $a\ne0$, the functions $1,X,X^2$ are independent on the interior. Their coefficients can match only if

$$
(\tfrac52-2a)(2-2a)=0,\qquad\boxed{a=1\ \text{or}\ a=\frac54}.
$$

Matching the remaining coefficients gives

$$
\dot\sigma=-15A\sigma^2,\qquad
 a\frac{\dot R}{R}=A\sigma\left[15-6(\tfrac52-a)(2-a)\right].
$$

Thus $\sigma=[15A(t+t_0)]^{-1}$, with $R=C(t+t_0)^{2/5}$ when $a=1$, and $R=C(t+t_0)^{1/2}$ when $a=5/4$. A nonzero solution whose support shrinks to zero at $t=0$ has $t_0=0$. The two [compact self-similar disk with density-linear viscosity](../../../../../../compact-self-similar-disk-with-density-linear-viscosity.md) profiles are consequently

$$
\boxed{\sigma(t)=\frac1{15At},\qquad
R(t)=\begin{cases}Ct^{2/5},&a=1,\\ Ct^{1/2},&a=5/4,\end{cases}\quad C>0, t>0}.
$$

Set $\Sigma=0$ for $r>R$. Both $r^{1/2}\bar\nu\Sigma$ and its first radial derivative vanish at the moving edge, because $\bar\nu\Sigma$ vanishes quadratically there. Together with $\Sigma(R)=0$, this makes the cutoff consistent with the diffusion equation without an added singular edge flux.

These are singular-origin [self-similar solutions](../../../../../../similarity-solution.md): $R(0)=0$ is a limiting support condition, while $\sigma$ diverges as $t\downarrow0$. It is not ordinary finite pointwise initial data. A finite nonzero $\sigma(0)$ would instead make $R=0$ an invariant solution of the radius equation, precluding an expanding nontrivial profile from that initial radius.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
