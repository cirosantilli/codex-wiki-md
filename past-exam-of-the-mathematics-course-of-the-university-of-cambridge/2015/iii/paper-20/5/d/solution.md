<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**Two successive point [blowups of a smooth algebraic surface](../../../../../../blowup-of-a-smooth-algebraic-surface.md) suffice.** Let $X_2\to X_1=\mathbb A^2$ be the [blowup of the affine plane at the origin](../../../../../../blowup-of-the-affine-plane-at-the-origin.md). In its chart $x=uy$, with coordinates $(y,u)$, the total-transform equation is

$$
x^2-y^5=y^2(u^2-y^3).
$$

Removing the exceptional factor gives the [strict transform](../../../../../../strict-transform.md)

$$
C_2:\ u^2-y^3=0.
$$

Above the original origin it has just one point, $(y,u)=(0,0)$, which is still singular. The other chart is $y=vx$, where the [strict transform](../../../../../../strict-transform.md) has equation $1-v^5x^3=0$ and does not meet the exceptional divisor $x=0$. Thus there are no other points above the origin to resolve.

Blow up the remaining point to obtain $X_3\to X_2$. In the chart $u=vy$, with coordinates $(y,v)$, the total transform of $C_2$ is

$$
u^2-y^3=y^2(v^2-y),
$$

and hence its [strict transform](../../../../../../strict-transform.md) is

$$
\boxed{C_3:\ y=v^2.}
$$

The derivative of $v^2-y$ with respect to $y$ is $-1$, so this is nonsingular, even in characteristics two or five. In the other chart $y=wu$, the [strict transform](../../../../../../strict-transform.md) has equation $1-w^3u=0$ and does not meet the exceptional divisor $u=0$. Therefore the only point of $C_3$ mapping to the original origin is the smooth point $(y,v)=(0,0)$.

The required sequence is

$$
\boxed{X_3=\operatorname{Bl}_{(0,0)}X_2\longrightarrow X_2=\operatorname{Bl}_0\mathbb A^2\longrightarrow X_1=\mathbb A^2.}
$$

The local parameter $v$ there gives $y=v^2$ and $x=v^5$, also verifying the resolved branch directly. This is the [resolution of the (2,5) cusp by two blowups](../../../../../../resolution-of-the-2-5-cusp-by-two-blowups.md). Its tangency to an exceptional divisor does not affect the requested nonsingularity of the [strict transform](../../../../../../strict-transform.md); making the whole total transform have normal crossings is a stronger task.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
