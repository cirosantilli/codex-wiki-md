<h1 id="34d/solution">Solution</h1>

↑ **Parent:** [34D](../34d.md)

Combining the real transformations gives

$$
F'_x=F_x,\qquad F'_y=\gamma(F_y+ivF_z),\qquad F'_z=\gamma(F_z-ivF_y).
$$

Let $v=\tanh\psi$, so $\gamma=\cosh\psi$ and $\gamma v=\sinh\psi$. The usual rotation about the positive $x$-axis has the $yz$ block $\left(\begin{smallmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{smallmatrix}\right)$. Taking $\boxed{n=(1,0,0),\ \theta=-i\psi}$ gives exactly the displayed transformation, because $\cos(-i\psi)=\cosh\psi$ and $\sin(-i\psi)=-i\sinh\psi$. This is a complex rotation, not a real spatial rotation.

Complex rotations preserve the bilinear dot product, without conjugation. Hence

$$
F\cdot F=E^2-B^2+2iE\cdot B
$$

is invariant, giving the two independent real [Lorentz invariants](../../../../../lorentz-invariance.md)

$$
\boxed{E^2-B^2,\qquad E\cdot B.}
$$

Their completeness refers to scalar invariants of the full [Lorentz group](../../../../../lorentz-group.md). For a generic non-null field, a boost along $E\times B$ makes the fields parallel. Indeed with $s=|E\times B|$ and $A=E^2+B^2$, the required speed solves $s(1+v^2)-Av=0$; the smaller root is $v=[A-\sqrt{(E^2-B^2)^2+4(E\cdot B)^2}]/(2s)<1$. For $s=0$ the fields are already parallel. A real rotation then gives $E=e n$, $B=b n$, leaving just $e^2-b^2$ and $eb$ as independent scalar parameters. Thus there are precisely two independent continuous scalar invariants on generic orbits; null fields have special orbits and the invariants do not distinguish zero from a nonzero null field.

If the printed phrase is read as invariance under only this single-axis boost, it admits extra fixed components $F_x$, so the assertion of precisely two must be understood in its Lorentz-scalar sense.

## ↑ Ancestors (10)

1. [34D](../34d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
