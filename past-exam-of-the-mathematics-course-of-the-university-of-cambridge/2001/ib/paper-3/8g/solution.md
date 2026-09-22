<h1 id="8g/solution">Solution</h1>

↑ **Parent:** [8G](../8g.md)

Take positive vortex strength $\kappa$ to mean anticlockwise [circulation](../../../../../circulation-physics.md). A [line vortex](../../../../../line-vortex.md) at $z_0$ has local [velocity potential](../../../../../velocity-potential.md) $\kappa\arg(z-z_0)/(2\pi)$. The [image vortex at a plane wall](../../../../../image-vortex-at-a-plane-wall.md) must have strength $-\kappa$ to enforce zero normal velocity at $y=0$. At the initial instant, a potential is therefore

$$
\boxed{\phi(x,y)=\frac{\kappa}{2\pi}\left[\arg((x-a)+i(y-b))-\arg((x-a)+i(y+b))\right].}
$$

This is a local, multivalued [velocity potential](../../../../../velocity-potential.md): its [gradient](../../../../../gradient.md) is single-valued away from the vortex, but the nonzero [circulation](../../../../../circulation-physics.md) precludes a globally single-valued potential around it. For a vortex centred at $(X,Y)$, the velocity is

$$
u_x=-\frac{\kappa}{2\pi}\frac{y-Y}{(x-X)^2+(y-Y)^2},\qquad
u_y=\frac{\kappa}{2\pi}\frac{x-X}{(x-X)^2+(y-Y)^2}.
$$

The real vortex and its opposite image give cancelling $u_y$ at the wall. A [point vortex](../../../../../line-vortex.md) moves with the regular velocity induced by the other vortex, not its singular self-field. Evaluating the image field at $(X,b)$ gives $\dot X=\kappa/(4\pi b)$ and $\dot b=0$. Hence

$$
\boxed{(X(t),Y(t))=\left(a+\frac{\kappa t}{4\pi b},\,b\right).}
$$

The time-dependent [velocity potential](../../../../../velocity-potential.md) is obtained by replacing $a$ with $X(t)$ above; the image remains at $(X(t),-b)$. Reversing the convention for positive [circulation](../../../../../circulation-physics.md) reverses the translation direction.

## ↑ Ancestors (10)

1. [8G](../8g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
