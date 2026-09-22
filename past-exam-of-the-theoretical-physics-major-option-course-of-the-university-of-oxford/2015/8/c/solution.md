<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Keep the index convention of [b](../b.md): $A^\mu=(A_0,\mathbf A)$, so $A_\mu=(A_0,-\mathbf A)$ and the spatial [gauge covariant derivative](../../../../gauge-covariant-derivative.md) is $\nabla+ie\mathbf A$. The physical three-current is the spatial part of $J^\mu$:

$$
\boxed{\mathbf j=ie(\varphi^*\nabla\varphi-\varphi\nabla\varphi^*)-2e^2|\varphi|^2\mathbf A.}
$$

Equivalently, writing $\varphi=R e^{i\theta}$ gives $\mathbf j=-2eR^2(\nabla\theta+e\mathbf A)$. Under the [gauge transformation](../../../../gauge-transformation.md) in [a](../a.md), $\theta\mapsto\theta+\alpha$ and $\mathbf A\mapsto\mathbf A-\nabla\alpha/e$, so this expression is manifestly invariant. Switching to a convention with the opposite spatial gauge sign reverses the phase-gradient term, not the screening term proportional to $e^2$.

For static fields the spatial [Ampère-Maxwell equation](../../../../ampere-s-circuital-law.md) is $\nabla\times\mathbf B=\mathbf j$, while $\nabla\cdot\mathbf B=0$. Taking its curl yields the general magnetic-field equation

$$
\boxed{\nabla^2\mathbf B=-\nabla\times\mathbf j
=-2ie\,\nabla\varphi^*\times\nabla\varphi
+2e^2\nabla|\varphi|^2\times\mathbf A
+2e^2|\varphi|^2\mathbf B.}
$$

No uniform-condensate approximation has yet been used. For a varying scalar amplitude the gradient terms must be kept; simply replacing $|\varphi|^2$ by a constant before deriving the current would conceal their origin. The homogeneous-condensate limit supplies the [London screening](../../../../london-screening.md) equation in [d](../d.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
