<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $E:y^2=x^3+x+1$, the duplication formula is

$$
x(2Q)=\frac{x(Q)^4-2x(Q)^2-8x(Q)+1}{4(x(Q)^3+x(Q)+1)}.
$$

At $P=(0,1)$, the tangent slope is $1/2$, so $x(2P)=1/4$ and $v_2(x(2P))=-2$. If $v_2(x(Q))=-2m<0$, the unique lowest-valuation terms in the numerator and denominator are respectively $x(Q)^4$ and $4x(Q)^3$, giving

$$
v_2(x(2Q))=-8m-(2-6m)=-2m-2.
$$

Induction yields $v_2(x(2^mP))=-2m$.

For a minimal integral equation, let $t=-x/y$ be the parameter of the [formal group of an elliptic curve](../../../../../../formal-group-of-an-elliptic-curve.md). Define

$$
E_r(\mathbb Q_p)=\{O\}\cup\{Q\in E_1(\mathbb Q_p):v_p(t(Q))\geq r\},
$$

where $E_1$ is the kernel of reduction to the identity. The parameter identifies $E_r$ with the formal group on $p^r\mathbb Z_p$. For odd $p$, the [formal logarithm](../../../../../../formal-logarithm.md) converges on $p\mathbb Z_p$ and is an analytic group isomorphism

$$
E_1(\mathbb Q_p)\cong p\mathbb Z_p\cong\mathbb Z_p.
$$

For $p=2$, the logarithm gives $E_2(\mathbb Q_2)\cong4\mathbb Z_2$. The formal duplication series satisfies $[2](T)=2T+O(T^3)$, so $[2](2u)/4\equiv u\pmod2$; successive lifting makes $[2]:E_1\to E_2$ surjective. Its kernel is rational 2-torsion, but $x^3+x+1$ has no root in $\mathbb Q_2$ because it has no root modulo $2$. Thus $[2]$ is an isomorphism and

$$
\boxed{E_1(\mathbb Q_2)\cong E_2(\mathbb Q_2)\cong\mathbb Z_2.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
