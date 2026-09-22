<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For unit vectors, the defining inequality for $Y$ is equivalent to $v\mathbin\cdot w\geq0$. Write

$$
w=tv+u,qquad u\in v^\perp=T_vS^{2n},qquad t\geq0.
$$

Then $t=(1-\lVert u\rVert^2)^{1/2}$, so

$$
(v,u)\longmapsto\bigl(v,(1-\lVert u\rVert^2)^{1/2}v+u\bigr)
$$

is a homeomorphism $D(TS^{2n})\to Y$. Replacing $v$ by $-v$ gives the same description of $Y'$. Their intersection is

$$
Z=\{(v,w):v\mathbin\cdot w=0\}=STS^{2n}=V_2(\mathbb R^{2n+1}),
$$

the [unit tangent bundle](../../../../../unit-tangent-bundle.md), equivalently a [Stiefel manifold](../../../../../stiefel-manifold.md). Since $e(TS^{2n})$ evaluates to $\chi(S^{2n})=2$, its Gysin sequence gives the [cohomology of the unit tangent bundle of an even-dimensional sphere](../../../../../cohomology-of-the-unit-tangent-bundle-of-an-even-dimensional-sphere.md):

$$
H^q(Z;\mathbb Z)\cong
\begin{cases}
\mathbb Z,&q=0,4n-1,\\
\mathbb Z/2,&q=2n,\\
0,&\text{otherwise}.
\end{cases}
$$

Every product of positive-degree classes vanishes.

Let $G$ consist of the eight signed permutations of the two factors:

$$
(v,w)\longmapsto(\varepsilon_1v,\varepsilon_2w)
\quad\text{or}\quad
(v,w)\longmapsto(\varepsilon_1w,\varepsilon_2v),
\qquad \varepsilon_i\in\{\pm1\}.
$$

It is the group of signed permutation matrices in dimension two, hence isomorphic to the [dihedral group](../../../../../dihedral-group.md) $D_8$, and every element preserves the equation $v\cdot w=0$. If $a,b$ generate $H^{2n}(X;\mathbb Z)$ from the two sphere factors, these maps act by the corresponding [signed permutation matrix](../../../../../signed-permutation-matrix.md), because the [antipodal map](../../../../../antipodal-map.md) of the even-dimensional sphere has degree $-1$. The eight actions are distinct, so only the identity can be homotopic to $1_X$.

Every element of $G$ acts trivially on $H^*(Z;\mathbb Z)$. The degree-$2n$ group is $\mathbb Z/2$, so its automorphism is forced to be the identity. On the top class, regard $Z$ as the [Stiefel manifold](../../../../../stiefel-manifold.md) of two-frames. The signed permutations are the right action of $O(2)$. The determinant-one component is connected, while a determinant-minus-one element is homotopic within that component to $(v,w)\mapsto(v,-w)$, the antipodal map on the $S^{2n-1}$ fibers. That map has degree $+1$, so the top class is also fixed.

The subgroup preserving $Y$ is

$$
H=\{1, AB, S, ABS\},
$$

where $A(v,w)=(-v,w)$, $B(v,w)=(v,-w)$, and $S(v,w)=(w,v)$. It consists exactly of the elements with $\varepsilon_1\varepsilon_2=1$. Under the deformation retraction $Y\simeq S^{2n}$ onto the diagonal, $1$ and $S$ act as the identity, while $AB$ and $ABS$ act as the antipodal map. They therefore act on $H^{2n}(Y;\mathbb Z)$ by $+1,+1,-1,-1$, respectively.

The [Thom isomorphism theorem](../../../../../thom-isomorphism-theorem.md) identifies $H^*(Y,Z)$ with a degree-$2n$ shift of $H^*(S^{2n})$. On the Thom class in degree $2n$, the same four elements act by $+1,+1,-1,-1$: the factor swap reverses each normal vector, which preserves the orientation because the normal rank $2n$ is even, while the simultaneous antipodal map reverses the oriented tangent fiber. On the degree-$4n$ relative class every element acts by $+1$, since the base and fiber signs for the last two elements cancel.

When $n=1$, $Z=V_2(\mathbb R^3)\cong SO(3)$. Every signed permutation of $(v,w)$ extends, after sending the third frame vector $v\times w$ to the required sign, to right multiplication by an element of $SO(3)$. Since $SO(3)$ is path-connected, every right translation is homotopic to the identity. Therefore

$$
\boxed{g|_Z\simeq1_Z\qquad\text{for every }g\in G.}
$$

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
