<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Translational and reflection symmetry parallel to the slabs imply $\mathbf E=E_x(x)\hat{\mathbf x}$. The differential [Gauss's law](../../../../gauss-s-law.md) is $dE_x/dx=\rho/\epsilon_0$. Starting at the left boundary with $E_x(-a)=0$ gives

$$
E_x(x)=-\frac{C}{\epsilon_0a}(x+a),\qquad -a\le x\le0.
$$

There is no singular [surface charge](../../../../surface-charge.md) at $x=0$, so the normal [electric field](../../../../electric-field-split.md) is continuous there: $E_x(0)=-C/\epsilon_0$. Integrating through the positive slab gives

$$
\boxed{\mathbf E(x)=\begin{cases}
-\dfrac{C(x+a)}{\epsilon_0a}\hat{\mathbf x},&-a\le x\le0,\\
-\dfrac{C(b-x)}{\epsilon_0b}\hat{\mathbf x},&0\le x\le b,\\
0,&x<-a\text{ or }x>b.
\end{cases}}
$$

The second expression indeed returns to zero at $x=b$, because the two total charges per unit area are $-C$ and $+C$. For $C>0$, the [electric field](../../../../electric-field-split.md) throughout the interior points from the positive slab towards the negative slab, along $-x$; reversing $C$ reverses the directions. The piecewise linear profile is a useful consequence of the uniform volume [charge density](../../../../charge-density.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
