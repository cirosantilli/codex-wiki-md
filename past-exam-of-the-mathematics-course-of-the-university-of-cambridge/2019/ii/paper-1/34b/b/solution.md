<h1 id="34b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Keep $\mathbf A=(0,Bx,0)$ and choose the [scalar potential](../../../../../../scalar-potential.md) $\phi=-Ex$. Then

$$
H=\frac1{2m}\left[p_x^2+(p_y-qBx)^2+p_z^2\right]-qEx.
$$

For $p_z=0$, completing the square gives

$$
H=\frac{p_x^2}{2m}
+\frac{m\omega_c^2}{2}(x-x_c)^2
-\frac EBp_y-\frac{mE^2}{2B^2},
\qquad
x_c=\frac{p_y}{qB}+\frac{mE}{qB^2}.
$$

Hence the spectrum on $\mathbb R^3$ is

$$
\boxed{E_n(k)=\hbar\omega_c\left(n+\frac12\right)
-\frac EB\hbar k-\frac{mE^2}{2B^2}.}
$$

For a translationally invariant dispersion, the [group velocity](../../../../../../group-velocity.md) is $v_y=\hbar^{-1}\partial E_n/\partial k$. Therefore

$$
\boxed{v_y=-\frac EB,}
$$

in agreement with the [electric-cross-magnetic-field drift](../../../../../../electric-cross-magnetic-field-drift.md) $\mathbf E\times\mathbf B/B^2$.

In the rectangle, $k=2\pi r/L_y$ as before. The energy now changes with $r$, so the guiding-centre degeneracy is lifted, while the number of states in each tilted band remains approximately $|qB|A/(2\pi\hbar)$. Adjacent states within a formerly degenerate level have the [electric-field splitting of a Landau level in a rectangle](../../../../../../electric-field-splitting-of-a-landau-level-in-a-rectangle.md)

$$
\boxed{\Delta E_{\rm electric}=\frac{2\pi\hbar}{L_y}\left|\frac EB\right|.}
$$

Thus this is the ground-to-first-excited gap when the lowest Landau band contains at least two allowed guiding centres and $\Delta E_{\rm electric}<\hbar\omega_c$. Without that implicit weak-field or large-sample condition, the exact full spectral gap is

$$
\boxed{\Delta E=\min\!\left\{\frac{2\pi\hbar|E|}{|B|L_y},\,\hbar\omega_c\right\}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [34B](../../34b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
