<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The diagram makes $x$ the remaining distance to the wall: $x$ decreases from $L$ to $0$. With the endpoint condition $m(0)=0$, integrating the supplied [mass](../../../../mass.md) gradient gives

$$
m(x)=\frac{Mx}{L}.
$$

Assume escaping sand has the same horizontal [velocity](../../../../velocity.md) as the bucket at release. There is then no horizontal recoil: the [momentum](../../../../momentum-split.md) flux of the outgoing sand cancels the $\dot m\dot x$ contribution to the bucket's [momentum](../../../../momentum-split.md) [derivative](../../../../derivative.md). The [variable-mass system](../../../../variable-mass-system.md) equation is therefore

$$
m\ddot x=-T.
$$

Set $u=-\dot x\ge0$, the [speed](../../../../speed.md) towards the wall. Since $\ddot x=u\,du/dx$, the initial condition $u(L)=0$ gives

$$
u\frac{du}{dx}=-\frac{TL}{Mx},\qquad
\boxed{u^2(x)=\frac{2TL}{M}\ln\frac Lx.}
$$

Consequently the remaining sand has [kinetic energy](../../../../kinetic-energy.md)

$$
\boxed{K(x)=\frac12m(x)u^2(x)=Tx\ln\frac Lx.}
$$

In terms of $z=x/L$, $K/(TL)=-z\ln z$. Its [derivative](../../../../derivative.md) is $-\ln z-1$ and its second [derivative](../../../../derivative.md) is $-1/z<0$, giving

$$
\boxed{x_K=\frac Le,\qquad K_{\max}=\frac{TL}{e}.}
$$

The magnitude of the remaining sand's [momentum](../../../../momentum-split.md) is

$$
\boxed{p(x)=m(x)u(x)=x\sqrt{\frac{2MT}{L}\ln\frac Lx}.}
$$

It is easier to maximize its square, $p^2/(2MTL)=-z^2\ln z$. Its [derivative](../../../../derivative.md) is $-z(2\ln z+1)$, giving the unique interior maximum

$$
\boxed{x_p=\frac L{\sqrt e},\qquad p_{\max}=\sqrt{\frac{MTL}{e}}.}
$$

Both [kinetic energy](../../../../kinetic-energy.md) and [momentum](../../../../momentum-split.md) tend to zero at $x\to0^+$, even though the idealized [speed](../../../../speed.md) diverges. There is no finite-[mass](../../../../mass.md) bucket left at the endpoint, so that divergence signals the limit of the idealization.

The [leaking bucket under constant tension](../../../../leaking-bucket-under-constant-tension.md) has $x_K=L/e<L/\sqrt e=x_p$: the [kinetic energy](../../../../kinetic-energy.md) maximum is closer to the wall. As the bucket loses [mass](../../../../mass.md), its increasing [speed](../../../../speed.md) continues to boost $K=pu/2$ after $p$ has begun to fall. Equivalently, $p\propto z\sqrt{-\ln z}$ and $K\propto z(-\ln z)$, so [kinetic energy](../../../../kinetic-energy.md) has the stronger dependence on the growing [speed](../../../../speed.md). The work $T(L-x)$ is shared between the remaining sand and the sand already lost; it is not all the bucket's instantaneous [kinetic energy](../../../../kinetic-energy.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [9](../../9.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the physics 1 paper of the University of Oxford](../../../split.md)
5. [Physics 1 paper of the University of Oxford](../../../../physics-1-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
