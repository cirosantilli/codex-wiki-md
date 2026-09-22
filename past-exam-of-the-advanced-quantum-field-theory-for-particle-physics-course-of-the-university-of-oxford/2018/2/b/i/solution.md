<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose an infinitesimal [gauge transformation](../../../../../gauge-transformation.md) $\delta A_\mu^a=D_\mu^{ab}\omega^b$, where $D_\mu^{ab}=\delta^{ab}\partial_\mu+g f^{acb}A_\mu^c$. Varying the axial gauge function at fixed $\sigma$ gives

$$
\delta f^a(x)=n^\mu D_\mu^{ab}\omega^b(x),\qquad
\boxed{M^{ab}(x,y)=n^\mu D_\mu^{ab}(x)\delta^{(4)}(x-y).}
$$

This is the [Faddeev-Popov operator](../../../../../faddeev-popov-operator.md). The [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) has a Grassmann representation $\det M\propto\int\mathcal D\bar c\,\mathcal Dc\,e^{i\int\bar cMc}$. Choosing this normalization for the antighost gives

$$
\boxed{\mathcal L_{\rm gh}=\bar c^a n\cdot\partial c^a
+g f^{acb}\bar c^a n^\mu A_\mu^c c^b.}
$$

A simultaneous antighost rephasing changes the overall ghost-action sign and vertex conventions, but not the determinant's field-dependent content. The essential facts are the kinetic operator $n\cdot\partial$ and a ghost-gluon vertex proportional to $n^\mu$.

Now average the fixed-$\sigma$ constraint with the stated Gaussian:

$$
\int\mathcal D\sigma\,\delta[n\cdot A-\sigma]
\exp\left[-\frac{i}{2\xi}\int d^4x\,\sigma^a\sigma^a\right]
=\exp\left[-\frac{i}{2\xi}\int d^4x\,(n\cdot A^a)^2\right]
$$

up to a field-independent normalization. Consequently

$$
\boxed{\mathcal L_{\rm gf}=-\frac1{2\xi}(n^\mu A_\mu^a)^2.}
$$

The [Faddeev-Popov ghost](../../../../../faddeev-popov-ghost.md) determinant is not generally field independent before imposing the strict axial condition: its interaction term contains $n\cdot A$. In the $\xi\to0$ gauge this quantity vanishes on the integration slice, giving the decoupling established next. Defining the inverse of $n\cdot\partial$ still requires boundary conditions for residual gauge transformations.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2018](../../../../2018-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
