<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Near $O$, put $t=-x/y$ and $w=-1/y$, or projectively $t=-X/Y$, $w=-Z/Y$. The integral [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md) becomes

$$
w=t^3+a_1tw+a_2t^2w+a_3w^2+a_4tw^2+a_6w^3.
$$

The linear coefficient of $w$ at the origin is a unit, so successive coefficient comparison gives a unique series $w(t)\in\mathbb Z_p[[t]]$ beginning $t^3$. Expressing the addition morphism in the local parameters of its two inputs gives

$$
F(t_1,t_2)=t_1+t_2+\text{terms of total degree at least two}\in\mathbb Z_p[[t_1,t_2]].
$$

Its identity, inverse, commutativity and associativity identities follow from the corresponding elliptic [group](../../../../../../group-split.md) identities. This one-dimensional commutative [formal group law](../../../../../../formal-group-law.md) is the [formal group of an elliptic curve](../../../../../../formal-group-of-an-elliptic-curve.md) $\widehat E$ attached to the model.

A point reducing to $O$ lies in the chart with $Y$ a unit and has $t,w\in p\mathbb Z_p$. The implicit equation determines $w$ uniquely from $t$. Conversely every $t\in p\mathbb Z_p$ gives the convergent solution $w(t)$ and the point $[-t:1:-w(t)]$; $t=0$ gives $O$. Hence the parameter is a bijection from the reduction kernel to $p\mathbb Z_p$. The series $F$ converges there and describes its addition. Therefore

$$
\boxed{\ker\varphi=E_1(\mathbb Q_p)\cong\widehat E(p\mathbb Z_p).}
$$

For nonzero $t$ with $v_p(t)=r>0$, $w(t)=t^3$ times a unit, so $v_p(x)=-2r$ and $v_p(y)=-3r$. These are the [formal kernel of a minimal Weierstrass equation](../../../../../../formal-kernel-of-a-minimal-weierstrass-equation.md) [valuations](../../../../../../valuation.md) used earlier.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
