<h1 id="s7/1/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $w=a^2\Omega^2/C$, requiring $C\ne0$ and $a>0$. The initial conditions fix $\ell=a^2\Omega$ and $\dot z=w+C\log(R/a)$. At $R=a$, the radial force is $a\Omega^2-Cw/a=0$. Thus the unperturbed motion is the helix

$$
\boxed{R=a,\qquad\phi=\Omega t,\qquad z=wt.}
$$

To analyse a small initial radial velocity, eliminate the cyclic velocities using the conserved quantities. The radial energy equation is $\dot R^2/2+U(R)=\mathcal E$, with

$$
U(R)=\frac{a^4\Omega^2}{2R^2}+\frac12\left[w+C\log(R/a)\right]^2.
$$

Here $U'(a)=0$ and $U''(a)=2\Omega^2+C^2/a^2>0$. The circular cylindrical radius is therefore stable. For $\eta=R-a$, the first-order equation is $\ddot\eta+\omega_r^2\eta=0$, so

$$
\boxed{\omega_r^2=2\Omega^2+\frac{C^2}{a^2},\qquad
R=a+\frac{\delta}{\omega_r}\sin\omega_rt+O(\delta^2).}
$$

The orbit acquires small radial oscillations. The other coordinates are modulated consistently with the same constants:

$$
\phi=\Omega t-\frac{2\Omega\delta}{a\omega_r^2}(1-\cos\omega_rt)+O(\delta^2),\qquad
z=wt+\frac{C\delta}{a\omega_r^2}(1-\cos\omega_rt)+O(\delta^2).
$$

These expressions retain the stated initial angular and axial velocities. The perturbation adds $\delta^2/2$ to the conserved energy. The expansion assumes $|\delta|/(a\omega_r)\ll1$, which follows from the supplied smallness condition when $\Omega\ne0$; it is not an exact finite-amplitude helix.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [1](../../1.md)
3. [S7](../../../s7.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
