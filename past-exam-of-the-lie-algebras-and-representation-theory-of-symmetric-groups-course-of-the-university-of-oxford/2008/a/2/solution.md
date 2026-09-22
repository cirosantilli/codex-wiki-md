<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Killing form](../../../../killing-form.md) is $\kappa_L(x,y)=\operatorname{tr}(\operatorname{ad}_Lx\,\operatorname{ad}_Ly)$. Symmetry follows from $\operatorname{tr}(AB)=\operatorname{tr}(BA)$. Since $\operatorname{ad}[z,x]=[\operatorname{ad}z,\operatorname{ad}x]$, cyclicity of [trace](../../../../matrix-trace.md) gives the invariance identity

$$
\kappa_L([z,x],y)=-\kappa_L(x,[z,y]).
$$

If $x\in I^\perp$ and $y\in I$, then $[z,y]\in I$, so the right side is zero. Hence $[z,x]\in I^\perp$ for every $z$, proving that $\boxed{I^\perp\text{ is an ideal}}$.

For $x\in I$, use a [basis](../../../../basis.md) of $I$ followed by a complementary [basis](../../../../basis.md) of $L$. Because $[x,L]\subseteq I$, the [matrix](../../../../matrix.md) of $\operatorname{ad}_Lx$ has blocks $\begin{pmatrix}\operatorname{ad}_Ix&B_x\\0&0\end{pmatrix}$. Multiplying two such [matrices](../../../../matrix.md) shows

$$
\boxed{\kappa_L(x,y)=\kappa_I(x,y)\quad(x,y\in I).}
$$

The restriction statement has both arguments in $I$; it does not identify the two forms for arbitrary elements of $L$ outside $I$.

Now use the ordered [basis](../../../../basis.md) in the question for a central [ideal](../../../../ideal-of-a-lie-algebra.md) $J$. The images of the $u_j$ in the quotient have adjoint [matrix](../../../../matrix.md) $A$, so the $u$-coordinate block of their images is $A$; arbitrary $J$-components form $B$. Each $v_j$ is central, so its image under every adjoint map is zero. Thus the [matrix](../../../../matrix.md) is exactly $\begin{pmatrix}A&0\\B&0\end{pmatrix}$. Products have top-left block $A_xA_y$ and zero bottom-right block. Taking traces gives

$$
\boxed{\kappa_L(x,y)=\kappa_{L/J}(\bar x,\bar y).}
$$

Finally, a nonzero finite-dimensional [nilpotent Lie algebra](../../../../nilpotent-lie-algebra.md) has nonzero [centre](../../../../center-of-a-lie-algebra.md) by (1)(b). Induct on its [dimension](../../../../dimension-vector-space.md): the [Killing form](../../../../killing-form.md) descends to the quotient by its [centre](../../../../center-of-a-lie-algebra.md), which is again nilpotent of smaller [dimension](../../../../dimension-vector-space.md), and is therefore zero by induction. The zero algebra starts the induction. Apply this to the nilpotent [ideal](../../../../ideal-of-a-lie-algebra.md) $I$ and then use the restriction identity to obtain $\boxed{\kappa_L(x,y)=0\text{ for }x,y\in I}$. This avoids the false general claim that the product of two nilpotent linear maps must be nilpotent.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../split.md)
5. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
