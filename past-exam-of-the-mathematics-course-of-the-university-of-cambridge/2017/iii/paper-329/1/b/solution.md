<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\mathbf e=\mathbf X/R$, $s=\mathbf e\cdot\mathbf B\mathbf e$, and $A_\parallel=\mathbf A\cdot\mathbf e$. Applied [forces](../../../../../../force.md) and couples below are [forces](../../../../../../force.md) and [torques](../../../../../../torque.md) on the solid; by [force](../../../../../../force.md) balance their values are also the strengths exerted by that solid on the fluid. This fixes the signs in [Faxén's first law](../../../../../../faxen-s-first-law.md) and [Faxén's rotational law](../../../../../../faxen-s-rotational-law.md). To hold the passive [sphere](../../../../../../sphere.md) fixed, set its translation and [angular velocity](../../../../../../angular-velocity.md) to zero in those laws. The incident [two-mode tensorial squirmer flow](../../../../../../two-mode-tensorial-squirmer-flow.md) gives

$$
\mathbf F_h=-6\pi\mu a\left(\mathbf u(\mathbf X)+\frac{a^2}{6}\nabla^2\mathbf u(\mathbf X)\right),\qquad
\mathbf G_h=-4\pi\mu a^3\boldsymbol\omega(\mathbf X).
$$

Only the [stresslet](../../../../../../force-dipole-flow.md) part has [vorticity](../../../../../../vorticity.md):

$$
\boldsymbol\omega(\mathbf x)=3a^2\frac{(\mathbf B\mathbf x)\times\mathbf x}{r^5}.
$$

Consequently, for fixed $\mathbf A,\mathbf B$ as $a/R\to0$,

$$
\boxed{\begin{aligned}\mathbf F_h&=-\frac{9\pi\mu a^3}{R^2}s\mathbf e
-\frac{2\pi\mu a^4}{R^3}(\mathbf A-3A_\parallel\mathbf e)
\\&\quad+O\!\left(\frac{\mu a^5\|\mathbf B\|}{R^4}+\frac{\mu a^8|\mathbf A|}{R^7}\right),\\
\mathbf G_h&=-\frac{12\pi\mu a^5}{R^5}(\mathbf B\mathbf X)\times\mathbf X+\text{higher reflections}.\end{aligned}}
$$

The leading [force](../../../../../../force.md) is the radial [stresslet](../../../../../../force-dipole-flow.md) [force](../../../../../../force.md). Its next correction, $O(\mu a^4|\mathbf A|/R^3)$, comes from the incident [potential dipole](../../../../../../potential-dipole.md). The next $\mathbf B$ correction, $O(\mu a^5\|\mathbf B\|/R^4)$, contains both the swimmer's $r^{-4}$ field and the [Laplacian](../../../../../../laplacian.md) term in [Faxén's first law](../../../../../../faxen-s-first-law.md). If the relevant coefficient vanishes, these next terms must be retained instead of calling the vanished term a nonzero leading approximation. Further exchanges in the [method of reflections for Stokes flow](../../../../../../method-of-reflections-for-stokes-flow.md) are smaller still.

The passive [sphere](../../../../../../sphere.md) reflects primarily a [Stokeslet](../../../../../../stokeslet.md) with strength $\mathbf F_h$. At the swimmer, its [velocity](../../../../../../velocity.md) is $(\mathbf I+\mathbf e\mathbf e)\mathbf F_h/(8\pi\mu R)$. The unchanged [surface slip velocity](../../../../../../surface-slip-velocity.md) adds the free swimming [velocity](../../../../../../velocity.md) to the incident-flow contribution in [Faxén's first law](../../../../../../faxen-s-first-law.md). Thus

$$
\boxed{\begin{aligned}\delta\mathbf U&=-\frac{9a^3}{4R^3}s\mathbf e
-\frac{a^4}{4R^4}(\mathbf A-5A_\parallel\mathbf e)
\\&\quad+O\!\left(\frac{a^5\|\mathbf B\|}{R^5}+\frac{a^6|\mathbf A|}{R^6}\right).\end{aligned}}
$$

The leading change is $O(a^3\|\mathbf B\|/R^3)$; its next correction is the displayed $O(a^4|\mathbf A|/R^4)$ term. Finite-radius [Faxén's first law](../../../../../../faxen-s-first-law.md) corrections, the passive [sphere](../../../../../../sphere.md)'s reflected [stresslet](../../../../../../force-dipole-flow.md), and its [rotlet](../../../../../../rotlet.md) contribute at order $a^5\|\mathbf B\|/R^5$ to translation.

For a [Stokeslet](../../../../../../stokeslet.md) at the origin,

$$
\mathbf u_F(\mathbf x)=\frac1{8\pi\mu}\left(\frac{\mathbf F}{r}+\frac{(\mathbf F\cdot\mathbf x)\mathbf x}{r^3}\right).
$$

The [curl](../../../../../../curl.md) of the first term is $\mathbf F\times\mathbf x/r^3$; that of the second is also $\mathbf F\times\mathbf x/r^3$, before multiplying by $1/(8\pi\mu)$. Hence $\boldsymbol\omega_F=\mathbf F\times\mathbf x/(4\pi\mu r^3)$. At the swimmer use displacement $-\mathbf X$. The leading $\mathbf B$ [force](../../../../../../force.md) is parallel to $\mathbf X$, so its [Stokeslet](../../../../../../stokeslet.md) has zero [vorticity](../../../../../../vorticity.md) there. This eliminates the putative $O(a^3\|\mathbf B\|/R^4)$ rotation. The [potential dipole](../../../../../../potential-dipole.md) itself has no [vorticity](../../../../../../vorticity.md), but the holding [force](../../../../../../force.md) it induces is not radial. Applying [Faxén's rotational law](../../../../../../faxen-s-rotational-law.md) to its reflected [Stokeslet](../../../../../../stokeslet.md) yields

$$
\boxed{\boldsymbol\Omega=\frac12\frac{\mathbf F_{h,A}\times(-\mathbf X)}{4\pi\mu R^3}
=\frac{a^4}{4R^6}\mathbf A\times\mathbf X
+O\!\left(\frac{a^5\|\mathbf B\|}{R^6}+\frac{a^6|\mathbf A|}{R^7}\right).}
$$

The passive [sphere](../../../../../../sphere.md)'s [rotlet](../../../../../../rotlet.md) and reflected [stresslet](../../../../../../force-dipole-flow.md) can affect that last order, so they cannot restore the larger missing rotation. When $\mathbf A\times\mathbf X=0$, the boxed coefficient is zero and the higher-order terms determine any rotation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
