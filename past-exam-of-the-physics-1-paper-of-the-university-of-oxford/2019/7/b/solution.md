<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The escaping sand initially has the bucket's [velocity](../../../../velocity.md), so it produces no relative-velocity thrust. This distinction is essential in a [leaking Atwood machine](../../../../leaking-atwood-machine.md). With upward [velocity](../../../../velocity.md) $v$ for the leaky side, the two bucket equations are

$$
M\dot v=T-Mg,\qquad M_0\dot v=M_0g-T.
$$

Their sum gives $\dot v=g(M_0-M)/(M+M_0)$. Since $\dot M=-\alpha$, it follows that

$$
\frac{dv}{dM}=\frac g\alpha\frac{M-M_0}{M+M_0}.
$$

Integrate from $M_0$, where the [velocity](../../../../velocity.md) is zero:

$$
v(M)=\frac g\alpha\left[M-M_0-2M_0\log\left(\frac{M+M_0}{2M_0}\right)\right].
$$

At emptying, $M=(1-\epsilon)M_0$, giving

$$
\boxed{v_{\rm empty}=\frac{gM_0}{\alpha}\left[-\epsilon-2\log(1-\epsilon/2)\right].}
$$

This is upward and positive for $0<\epsilon<1$. For no initial sand, $\epsilon=0$, the emptying time is zero and the [speed](../../../../speed.md) is zero. As the dry bucket [mass](../../../../mass.md) tends to zero,

$$
\boxed{\lim_{\epsilon\to1^-}v_{\rm empty}=\frac{gM_0}{\alpha}(2\log2-1).}
$$

This finite limit refers to the idealized model; the endpoint itself would describe a massless empty bucket. For small $\epsilon$, $v_{\rm empty}\sim gM_0\epsilon^2/(4\alpha)$, consistent with initially zero [acceleration](../../../../acceleration.md) that grows as [mass](../../../../mass.md) is lost.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the physics 1 paper of the University of Oxford](../../../split.md)
5. [Physics 1 paper of the University of Oxford](../../../../physics-1-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
