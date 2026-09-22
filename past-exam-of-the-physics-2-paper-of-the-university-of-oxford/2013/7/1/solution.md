<h1 id="7/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The upper positive plate gives a downward field $E=V/a$, while $\mathbf B$ points into the page. For a rightward electron, the electric force is upward and the magnetic force downward. Its initial speed is

$$
v_0=\sqrt{\frac{2(1\,\mathrm{eV})}{m_e}}=5.931\times10^5\,\mathrm{m\,s^{-1}},\qquad
\frac EB=\frac{20000}{0.0337(1)}=5.935\times10^5\,\mathrm{m\,s^{-1}}.
$$

These are equal to the precision intended by the rounded plate spacing: the arrangement is a [velocity selector](../../../../velocity-selector.md). Accordingly,

$$
\boxed{\theta_{\rm exit}\simeq0.}
$$

It is not appropriate to calculate a large electric deflection and ignore magnetic bending. For completeness, if all printed values are treated literally, let $v_d=E/B$, $u=v_0-v_d$, and $\omega_c=eB/m_e$. The exact nonrelativistic crossed-field motion is

$$
x=v_dt+\frac{u}{\omega_c}\sin\omega_ct,\qquad y=\frac{u}{\omega_c}(\cos\omega_ct-1),
$$

with $v_x=v_d+u\cos\omega_ct$ and $v_y=-u\sin\omega_ct$. At the exit solve $x(t_e)=0.50$ m, then use $\theta=\operatorname{atan2}(v_y,v_x)$. The small rounding mismatch produces nanometre-scale oscillations, with $|\theta|\le\sin^{-1}(|u|/v_d)\simeq6.32\times10^{-4}$ rad. Its precise oscillatory exit angle is not robust to the supplied rounding.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [7](../../7.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
