<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Electrical contact equalizes [electric potential](../../../../electric-potential.md) and preserves total [electric charge](../../../../electric-charge-split.md). **The usual isolated-sphere approximation** assigns the two [conducting spheres](../../../../conducting-sphere.md) the [capacitances](../../../../capacitance.md) $4\pi\epsilon_0R$ and $8\pi\epsilon_0R$. It then gives

$$
\frac{Q_R}{R}=\frac{Q_{2R}}{2R},\qquad Q_R+Q_{2R}=Q,
\qquad \boxed{Q_R\simeq Q/3,\quad Q_{2R}\simeq2Q/3.}
$$

These are accurate when the [conducting spheres](../../../../conducting-sphere.md) are far apart and joined by a thin wire. **Literal touching changes the answer:** each [conducting sphere](../../../../conducting-sphere.md) polarizes the other, so its [electric potential](../../../../electric-potential.md) is not its isolated value. The source does not specify an approximation which would remove this effect.

For completeness, the exact result for ideal externally tangent [conducting spheres](../../../../conducting-sphere.md) can be obtained by the [method of images](../../../../method-of-images.md). Let their radii be $a,b$, their centre separation $D=a+b$, and their common [electric potential](../../../../electric-potential.md) $V$. Begin with central [image charges](../../../../image-charge.md) $4\pi\epsilon_0Va$ and $4\pi\epsilon_0Vb$. Reflect each external [image charge](../../../../image-charge.md) $q'$ at centre-distance $s$ into the other [conducting sphere](../../../../conducting-sphere.md) of radius $a$: the new [image charge](../../../../image-charge.md) is $-a q'/s$ at centre-distance $a^2/s$ toward the original. Repeat, alternately, in the two [conducting spheres](../../../../conducting-sphere.md). Pairing successive opposite-sign terms gives the convergent net [electric charges](../../../../electric-charge-split.md)

$$
\begin{aligned}
Q_a&=4\pi\epsilon_0Vab\sum_{n=0}^{\infty}\left(\frac1{b+nD}-\frac1{(n+1)D}\right),\\
Q_b&=4\pi\epsilon_0Vab\sum_{n=0}^{\infty}\left(\frac1{a+nD}-\frac1{(n+1)D}\right).
\end{aligned}
$$

Each reflection cancels a nonconstant surface [electric potential](../../../../electric-potential.md); the remaining central term fixes $V$. The total internal [image charge](../../../../image-charge.md) equals the exterior [electric flux](../../../../electric-flux.md) divided by $1/\epsilon_0$, so these sums give the physical net [electric charges](../../../../electric-charge-split.md).

For $a=R,b=2R$, multiply both dimensionless sums by the common factor $4\pi\epsilon_0V(2R/3)$. Their values follow by writing reciprocals as [integrals](../../../../integral-split.md) and setting $t=u^3$:

$$
\begin{aligned}
S_a&=\sum_{n=0}^{\infty}\left(\frac1{n+2/3}-\frac1{n+1}\right)=3\int_0^1\frac{u\,du}{1+u+u^2}=\frac32\ln3-\frac{\pi}{2\sqrt3},\\
S_b&=\sum_{n=0}^{\infty}\left(\frac1{n+1/3}-\frac1{n+1}\right)=3\int_0^1\frac{(1+u)\,du}{1+u+u^2}=\frac32\ln3+\frac{\pi}{2\sqrt3}.
\end{aligned}
$$

Dividing by $S_a+S_b$ enforces [conservation of electric charge](../../../../charge-conservation.md) and yields

$$
\boxed{Q_R=Q\left(\frac12-\frac{\pi}{6\sqrt3\ln3}\right)\simeq0.22483Q,\qquad Q_{2R}=Q\left(\frac12+\frac{\pi}{6\sqrt3\ln3}\right)\simeq0.77517Q.}
$$

This concrete touching-sphere result disproves applying the isolated $1:2$ sharing rule to literal contact.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
