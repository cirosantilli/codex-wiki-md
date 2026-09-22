<h1 id="32e/solution">Solution</h1>

↑ **Parent:** [32E](../32e.md)

Write $\xi=V_1$ and $\eta=\phi$. The vector field

$$
V=\xi(x,u)\partial_x+\eta(x,u)\partial_u
$$

generates a [Lie point symmetry of an ordinary differential equation](../../../../../lie-point-symmetry-of-an-ordinary-differential-equation.md) if its local flow maps solution graphs to solution graphs. Its $n$th [prolongation of a vector field](../../../../../prolongation-of-a-vector-field.md) is

$$
\operatorname{pr}^{(n)}V
=V+\sum_{j=1}^n\eta^{(j)}\partial_{u^{(j)}},
$$

where

$$
\eta^{(0)}=\eta,
\qquad
\eta^{(j)}=D_x\eta^{(j-1)}-u^{(j)}D_x\xi
$$

and

$$
D_x=\partial_x+u'\partial_u+u''\partial_{u'}+\cdots
$$

is the [total derivative operator](../../../../../total-derivative-operator.md). The infinitesimal invariance criterion is

$$
\boxed{
\operatorname{pr}^{(n)}V(\Delta)=0
\quad\text{whenever }\Delta=0
}.
$$

Put $p=u'$ and $q=u''$. Direct calculation gives

$$
\eta^{(1)}
=\eta_x+(\eta_u-\xi_x)p-\xi_up^2
$$

and

$$
\eta^{(2)}
=\eta_{xx}+(2\eta_{xu}-\xi_{xx})p
+(\eta_{uu}-2\xi_{xu})p^2-\xi_{uu}p^3
+(\eta_u-2\xi_x-3\xi_up)q.
$$

For

$$
\Delta=q-\frac{p^2}{u}+u^2,
$$

the invariance condition is

$$
\eta^{(2)}
-\frac{2p}{u}\eta^{(1)}
+\frac{p^2}{u^2}\eta
+2u\eta=0
$$

after imposing $q=p^2/u-u^2$. The coefficient of $p^3$ is

$$
-\xi_{uu}-\frac1u\xi_u.
$$

It must vanish identically, so

$$
\partial_u(u\xi_u)=0.
$$

Since $u>0$, integration gives

$$
\boxed{\xi(x,u)=F(x)\log u+G(x)}
$$

for functions $F,G$.

Now take

$$
\xi=cx+d,
\qquad
\eta=-2cu.
$$

Then

$$
\eta^{(1)}=-3cp,
\qquad
\eta^{(2)}=-4cq,
$$

and substitution gives

$$
\operatorname{pr}^{(2)}V(\Delta)
=-4c\left(q-\frac{p^2}{u}+u^2\right)
=-4c\Delta.
$$

Thus the infinitesimal invariance criterion holds.

The generated one-parameter transformation is, for $c\ne0$,

$$
\boxed{
\widetilde x=e^{c\varepsilon}\left(x+\frac dc\right)-\frac dc,
\qquad
\widetilde u=e^{-2c\varepsilon}u
},
$$

while for $c=0$ it is $\widetilde x=x+d\varepsilon$, $\widetilde u=u$. Combining these transformations gives the two-parameter symmetry group

$$
\boxed{
(x,u)\longmapsto(\lambda x+a,\lambda^{-2}u),
\qquad \lambda>0,\ a\in\mathbb R
}.
$$

This is the [affine-scaling symmetry of u double prime equals u prime squared over u minus u squared](../../../../../affine-scaling-symmetry-of-u-double-prime-equals-u-prime-squared-over-u-minus-u-squared.md).

## ↑ Ancestors (10)

1. [32E](../32e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
