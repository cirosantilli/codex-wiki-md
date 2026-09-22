<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Identify the ambient real four-dimensional vector space with $2\times2$ real matrices by

$$
X(u,v,x,y)=\begin{pmatrix}u+x&y+v\\y-v&u-x\end{pmatrix},\qquad
-\det X=-u^2-v^2+x^2+y^2.
$$

For $A,B\in SL(2,\mathbb R)$, the linear action $X\mapsto AXB^{-1}$ preserves this quadratic form. It gives a group homomorphism to the [special orthogonal group](../../../../../special-orthogonal-group.md) of signature $(2,2)$; its determinant on matrix space is $(\det A)^2(\det B)^{-2}=1$. The group $SL(2,\mathbb R)$ is connected: an oriented Gram–Schmidt factorization writes every element as a rotation times an upper triangular matrix with positive diagonal and determinant one, and each factor varies in a connected space. Thus the image lies in the identity component $SO_0(2,2)$.

If $AXB^{-1}=X$ for every $X$, taking $X=I$ gives $A=B$. A matrix commuting with every real $2\times2$ matrix is scalar, and its determinant-one condition then gives $A=B=\pm I$. The kernel is therefore exactly $\{(I,I),(-I,-I)\}$. Infinitesimally the action is $X\mapsto aX-Xb$, with $a,b$ traceless. If this vanishes for every $X$, then $a=b$ and it is scalar and traceless, hence zero. The differential is injective; source and target [Lie algebras](../../../../../lie-algebra-split.md) each have dimension six, so it is an isomorphism. The image is therefore an open subgroup of the connected target, which must be the entire target. Consequently

$$
\boxed{SO_0(2,2)\cong\frac{SL(2,\mathbb R)\times SL(2,\mathbb R)}{\{(I,I),(-I,-I)\}}.}
$$

The finite quotient is by the diagonal central subgroup, not by a sign in just one factor. The connected-component subscript is a genuine qualification of the source's displayed formula: the full $SO(2,2)$ is disconnected and cannot be isomorphic to a quotient of the connected product.

Let the anti-de Sitter radius be $\ell>0$. Its quadric is $-u^2-v^2+x^2+y^2=-\ell^2$, or $\det X=\ell^2$. Thus the map $X\mapsto g=X/\ell$ identifies this quadric smoothly and globally with $SL(2,\mathbb R)$. This is the [group model of three-dimensional anti-de Sitter spacetime](../../../../../group-model-of-three-dimensional-anti-de-sitter-spacetime.md). The induced [Lorentzian metric](../../../../../lorentzian-metric.md) is bi-invariant, since the two matrix multiplication actions preserve the ambient quadratic form. At the identity, tangent matrices $a,b$ are traceless and

$$
g_\ell(a,b)=\frac{\ell^2}{2}\operatorname{Tr}(ab).
$$

Indeed, for a traceless matrix $a$, $\det a=-\frac12\operatorname{Tr}(a^2)$, and polarizing $-\det(\ell a)$ gives this metric. For $\mathfrak{sl}_2(\mathbb R)$ the [Killing form](../../../../../killing-form.md) is $K(a,b)=4\operatorname{Tr}(ab)$: in the basis $H=\operatorname{diag}(1,-1)$, $E=\begin{pmatrix}0&1\\0&0\end{pmatrix}$ and $F=\begin{pmatrix}0&0\\1&0\end{pmatrix}$, the brackets are $[H,E]=2E$, $[H,F]=-2F$, $[E,F]=H$, giving $K(H,H)=8$, $K(E,F)=4$ and the remaining independent pairings zero. Therefore $g_\ell=\ell^2K/8$.

The [canonical torsion-free connection on a Lie group](../../../../../canonical-torsion-free-connection-on-a-lie-group.md) is the [Levi-Civita connection](../../../../../levi-civita-connection.md) of this [bi-invariant pseudo-Riemannian metric](../../../../../bi-invariant-pseudo-riemannian-metric.md). Its [Ricci tensor](../../../../../ricci-tensor.md), already calculated from the double bracket, is

$$
\boxed{\operatorname{Ric}=-\frac14K=-\frac2{\ell^2}g_\ell,\qquad R=-\frac6{\ell^2}.}
$$

Substitution into the vacuum [Einstein field equations](../../../../../einstein-field-equations.md) gives

$$
\operatorname{Ric}-\frac12Rg_\ell+\Lambda g_\ell
=\left(\frac1{\ell^2}+\Lambda\right)g_\ell=0,
\qquad \boxed{\Lambda=-\ell^{-2}.}
$$

Thus the group metric solves the three-dimensional vacuum equations with negative [cosmological constant](../../../../../cosmological-constant.md).

The antipodal map $X\mapsto-X$ is $g\mapsto-g$, multiplication by the central element $-I$. Hence **the antipodal quotient is $PSL(2,\mathbb R)=SL(2,\mathbb R)/\{\pm I\}$**, with the same local curvature and cosmological constant. To see the global time issue, use

$$
u=\ell\cosh\rho\cos t,\quad v=\ell\cosh\rho\sin t,\quad
x=\ell\sinh\rho\cos\varphi,\quad y=\ell\sinh\rho\sin\varphi.
$$

The induced metric is

$$
ds^2=\ell^2\bigl(-\cosh^2\rho\,dt^2+d\rho^2+\sinh^2\rho\,d\varphi^2\bigr).
$$

On the quadric $t$ has period $2\pi$; curves with fixed $\rho,\varphi$ are closed timelike curves. The antipodal identification is $(t,\varphi)\sim(t+\pi,\varphi+\pi)$, and does not eliminate this problem. At $\rho=0$, even the half-period time shift closes after the antipodal quotient.

If global time is not identified, take the [universal cover](../../../../../universal-cover.md), with $t\in\mathbb R$. The topology of $SL(2,\mathbb R)$ is $S^1\times\mathbb R^2$, as follows from the same rotation–triangular decomposition, so the universal cover is diffeomorphic to $\mathbb R^3$ and carries the lifted group structure $\widetilde{SL(2,\mathbb R)}$. The metric and Einstein equation are unchanged locally. Here $t$ is a global time function with timelike gradient, excluding closed causal curves. **Unwrapped anti-de Sitter spacetime is the universal covering group, rather than the original embedded quadric or its antipodal quotient**; retaining the antipodal time-shift identification would wrap time again.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 65](../../paper-65-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
