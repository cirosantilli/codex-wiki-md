<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Killing form](../../../../killing-form.md) is $\kappa_L(x,y)=\operatorname{Tr}(\operatorname{ad}x\operatorname{ad}y)$. Write $X=\operatorname{ad}x$, $Y=\operatorname{ad}y$, $Z=\operatorname{ad}z$. Since $\operatorname{ad}[x,y]=[X,Y]$, cyclicity of [trace](../../../../matrix-trace.md) gives

$$
\kappa_L([x,y],z)=\operatorname{Tr}((XY-YX)Z)=\operatorname{Tr}(X(YZ-ZY))=\kappa_L(x,[y,z]).
$$

If $x\in I^\perp$, $a\in L$ and $y\in I$, invariance gives $\kappa_L([a,x],y)=\kappa_L(x,[y,a])=0$, because $[y,a]\in I$. Thus **$I^\perp$ is an ideal**. For $x,y\in I$, the restrictions of their adjoint maps to $I$ are the adjoint maps of $I$, and their induced maps on $L/I$ vanish. Block traces therefore give $\kappa_L|_{I\times I}=\kappa_I$.

If $A$ is an Abelian ideal, $\operatorname{ad}a\operatorname{ad}x$ maps $L$ into $A$ and vanishes on $A$ for $a\in A$. In a [basis](../../../../basis.md) starting with $A$ it has zero diagonal blocks, hence [trace](../../../../matrix-trace.md) zero. Therefore **every Abelian ideal lies in $L^\perp$**.

[Cartan criterion for semisimplicity](../../../../cartan-criterion-for-semisimplicity.md) says that a finite-dimensional complex [Lie algebra](../../../../lie-algebra-split.md) is semisimple exactly when its [Killing form](../../../../killing-form.md) is nondegenerate. To see why nondegeneracy implies semisimplicity, any nonzero solvable ideal has a last nonzero derived term which is an Abelian ideal of $L$. The previous paragraph would put it in the radical of the [Killing form](../../../../killing-form.md), a contradiction.

If $L$ is a semisimple ideal of $M$, the restriction $\kappa_M|_L=\kappa_L$ is nondegenerate. Put $J=L^{\perp_{\kappa_M}}$. This is an ideal of $M$ by the argument above, and nondegeneracy on $L$ gives $L\cap J=0$ and $M=L+J$. One way to check the latter is to restrict the pairing map $M\to L^*$: its restriction to $L$ is an isomorphism, so every vector of $M$ can be adjusted by an element of $L$ to lie in its kernel $J$. Since both are ideals, $[L,J]\subseteq L\cap J=0$. Hence

$$
\boxed{M=L\oplus J\text{ as a direct sum of ideals}.}
$$

Apply this to the supplied extension by the derivation. If $\delta=0$, it is $\operatorname{ad}0$. Otherwise $D$ and $J$ are one-dimensional, and projection $J\to D$ is an isomorphism. Choose its vector with $D$-component $\delta$, writing it as $j=\delta-x$ for $x\in L$. Because $[J,L]=0$, for every $l\in L$ one has $0=[j,l]=\delta(l)-[x,l]$. Thus

$$
\boxed{\delta=\operatorname{ad}_Lx.}
$$

This also handles the sign in the extension bracket explicitly.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../split.md)
5. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
