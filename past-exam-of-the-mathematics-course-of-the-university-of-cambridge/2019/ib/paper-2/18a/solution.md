<h1 id="18a/solution">Solution</h1>

↑ **Parent:** [18A](../18a.md)

For a moving circuit, [Faraday's law](../../../../../faraday-s-law-of-induction.md) states that the [electromotive force](../../../../../electromotive-force.md)

$$
\mathcal E=\oint_C(\mathbf E+\mathbf v\times\mathbf B)\cdot d\boldsymbol\ell
$$

equals $-d\Phi_B/dt$, where $\Phi_B=\int_S\mathbf B\cdot d\mathbf S$ is the [magnetic flux](../../../../../magnetic-flux.md) through any spanning surface. Choose the upward normal. The horizontal square has

$$
\Phi_B=(-2bz)(2a)^2=-8ba^2z,
$$

so [Ohm's law](../../../../../ohm-s-law.md) gives the induced current

$$
\boxed{I=\frac{\mathcal E}{R}=\frac{8ba^2}{R}\dot z}
$$

with positive current taken counterclockwise from above.

On the edge $x=a$, $d\boldsymbol\ell=dy\,\mathbf e_y$. The [magnetic force on a current-carrying wire](../../../../../magnetic-force-on-a-current-carrying-wire.md) is $d\mathbf F=I,d\boldsymbol\ell\times\mathbf B$, hence

$$
\mathbf F_{x=a}
=Ib\int_{-a}^a\mathbf e_y\times(a\mathbf e_x+y\mathbf e_y-2z\mathbf e_z)\,dy
=\boxed{-4abIz\,\mathbf e_x-2a^2bI\,\mathbf e_z}.
$$

The ratio of the horizontal to vertical magnitudes is $2|z|/a$, so the directed force makes angle $\tan^{-1}(2z/a)$ with the vertical, with the sign fixing the horizontal side.

The horizontal forces on opposite edges cancel, while all four vertical contributions add:

$$
\boxed{\mathbf F_{\rm em}=-8ba^2I\,\mathbf e_z
=-\frac{(8ba^2)^2}{R}\dot z\,\mathbf e_z}.
$$

This is an electromagnetic drag force opposing the motion, as required by [Lenz's law](../../../../../lenz-s-law.md). Including gravity gives

$$
m\ddot z=-mg-\frac{(8ba^2)^2}{R}\dot z.
$$

At the [terminal velocity](../../../../../terminal-speed-of-a-falling-conducting-loop.md), $\ddot z=0$, and the constant downward speed has magnitude

$$
\boxed{v_{\rm terminal}=\frac{Rmg}{(8ba^2)^2}}.
$$

## ↑ Ancestors (10)

1. [18A](../18a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
