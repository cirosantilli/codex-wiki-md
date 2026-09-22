<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A representative of an element of $G$ is a determinant-one matrix $\left(\begin{smallmatrix}a&b\\\overline b&\overline a\end{smallmatrix}\right)$ over the [Gaussian integers](../../../../../gaussian-integer.md), considered up to its common sign. It acts by a [Möbius transformation](../../../../../mobius-transformation.md) of the disk. Since $T(0)=b/\overline a$ and $|a|^2-|b|^2=1$, we have

$$
|a|^2=\frac1{1-|T(0)|^2}.
$$

Only finitely many Gaussian-integer pairs $(a,b)$ can have $T(0)$ in a fixed compact subdisk. More generally, if $T$ carries some point of a compact set $K$ into $K$, and $K$ lies in the hyperbolic ball of radius $R$ about zero, the [triangle inequality](../../../../../triangle-inequality.md) gives $\rho(0,T0)\leq2R$. Thus there are only finitely many such $T$. This proves the [properly discontinuous group action](../../../../../properly-discontinuous-group-action.md), and in particular discreteness. The specified $A,B$ belong to $G$, so their subgroup $H$ is discrete as well.

The fixed-point equations reduce to $-i(z-1)^2=0$ for $A$ and $i(z+1)^2=0$ for $B$. Thus their unique fixed points are respectively $1$ and $-1$ on the ideal boundary. Neither transformation is the identity; their displayed determinant-one representatives have trace two. They are therefore [parabolic Möbius transformations](../../../../../parabolic-element-of-psl2-r.md).

To find the [Dirichlet domains](../../../../../dirichlet-domain.md), use the [Möbius transformation](../../../../../mobius-transformation.md)

$$
C(z)=i\frac{1+z}{1-z},\qquad C(0)=i.
$$

It takes the disk to the upper half-plane, and direct substitution gives

$$
CAC^{-1}(w)=w-2,\qquad CBC^{-1}(w)=\frac{w}{2w+1}.
$$

For $w=x+iy$ and $v$ in the upper half-plane, the [hyperbolic distance](../../../../../hyperbolic-distance.md) obeys $\cosh\rho(w,v)=1+|w-v|^2/(2y\operatorname{Im}v)$. Since $C(A^k0)=i-2k$, the distance inequalities are equivalent to

$$
x^2+(y-1)^2\leq(x+2k)^2+(y-1)^2\quad(k\in\mathbb Z).
$$

These reduce to $kx+k^2\geq0$ for all integers $k$. The cases $k=1,-1$ imply $-1\leq x\leq1$, which also suffices for every other $k$. Therefore the cyclic [Dirichlet domain](../../../../../dirichlet-domain.md) becomes the strip $|\operatorname{Re}w|\leq1$.

The two vertical [hyperbolic geodesics](../../../../../geodesic-in-the-poincare-half-plane-model.md) pull back to arcs joining $1$ to $i$ and $1$ to $-i$. In disk coordinates they are the circles $|z-(1+i)|=1$ and $|z-(1-i)|=1$, restricted to the disk. Thus

$$
\boxed{D_A=\{z\in\mathbb D:|z-(1+i)|\geq1,\ |z-(1-i)|\geq1\}.}
$$

Conjugating by $z\mapsto-z$ gives $B$, so its two [hyperbolic geodesics](../../../../../geodesic-in-the-poincare-half-plane-model.md) join $-1$ to $i$ and $-1$ to $-i$, and

$$
\boxed{D_B=\{z\in\mathbb D:|z-(-1+i)|\geq1,\ |z-(-1-i)|\geq1\}.}
$$

The requested drawing and their intersection are shown below.

<a id="4/image-cyclic-parabolic-dirichlet-region-and-the-four-sided-region-for-the-two-generators"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-11-dirichlet-regions.png)

**[Figure 1](#4/image-cyclic-parabolic-dirichlet-region-and-the-four-sided-region-for-the-two-generators). Cyclic parabolic Dirichlet region and the four-sided region for the two generators**.

For any $z_0$, the orbit points satisfying $\rho(0,Tz_0)\leq\rho(0,z_0)$ form a nonempty finite set, by proper discontinuity and compactness of closed hyperbolic balls. Choose a closest one, $q=Tz_0$. For every integer $k$, its minimality gives

$$
\rho(0,q)\leq\rho(0,A^{-k}q)=\rho(A^k0,q),
$$

and the same inequality with $B$. Hence $q$ lies in the [ideal hyperbolic quadrilateral](../../../../../ideal-hyperbolic-quadrilateral.md)

$$
\boxed{P=D_A\cap D_B=\{z\in\mathbb D:|z-(\varepsilon+i\eta)|\geq1\text{ for }\varepsilon,\eta\in\{1,-1\}\}.}
$$

Its ideal vertices are $1,i,-1,-i$.

For the quotient identification, it remains to justify that this covering region is a fundamental polygon. The four open corner caps excluded by $P$ are pairwise disjoint inside the disk. The transformation $A$ carries the exterior of the lower-right cap into the upper-right cap; $A^{-1}$ reverses the pairing. Similarly $B$ carries the exterior of the upper-left cap into the lower-left cap, and $B^{-1}$ reverses this. These assertions follow either from the upper-half-plane formulas or by mapping their boundary circles and testing zero: $A0=(1+i)/2$ and $B0=(-1-i)/2$.

Apply a reduced word in $A^{\pm1},B^{\pm1}$ from right to left to a point in the interior of $P$. The first letter puts it into its target cap. Every subsequent letter can do the same, since its inverse cap is distinct from the preceding target cap unless the word cancels. Thus the final point lies in the target cap of the leftmost letter, never in the interior of $P$. This [ping-pong lemma](../../../../../ping-pong-lemma.md) argument proves freeness and disjointness of distinct translated interiors. Together with orbit coverage it makes $P$ a fundamental polygon. The corresponding argument on closed caps shows that boundary identifications are generated by the stated side pairings.

The generator $A$ pairs the side from $1$ to $-i$ with the side from $1$ to $i$, fixing the ideal endpoint $1$ and sending $-i$ to $i$. The generator $B$ pairs the side from $-1$ to $i$ with the side from $-1$ to $-i$, fixing $-1$ and sending $i$ to $-i$. There are three ideal-vertex classes: $\{1\}$, $\{-1\}$ and $\{i,-i\}$. The first two give parabolic ends from $A,B$; the third does too, since $AB$ is a nonidentity parabolic transformation fixing $i$. Adding one point at each end produces an oriented closed surface with one face, two edges and three vertices. Its [Euler characteristic](../../../../../euler-characteristic.md) is $1-2+3=2$, so it is a sphere. Removing the three added points gives a [thrice-punctured sphere](../../../../../thrice-punctured-sphere.md), proving

$$
\boxed{\mathbb D/H\text{ is homeomorphic to a thrice-punctured sphere}.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
