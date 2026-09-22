<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use $D_x=\partial_x+A_x$, $D_y=\partial_y+A_y$, acting on columns. Expanding the two compositions and cancelling their ordinary [derivative](../../../../../derivative.md) terms gives

$$
[D_x,D_y]v=(\partial_xA_y-\partial_yA_x+[A_x,A_y])v=F_{xy}v.
$$

Compatibility means local solvability for arbitrary initial vectors, equivalently the existence of an invertible parallel [bundle frame](../../../../../frame-of-a-vector-bundle.md) $S$ with $D_xS=D_yS=0$. Such a [bundle frame](../../../../../frame-of-a-vector-bundle.md) gives $F_{xy}S=0$, hence $F_{xy}=0$. A single specified parallel vector only implies $F_{xy}v=0$: for example $A_x=0$, $A_y=x\operatorname{diag}(1,0)$ and $v=(0,1)^T$ have $D_xv=D_yv=0$ although $F_{xy}=\operatorname{diag}(1,0)\ne0$. This is why arbitrary-data compatibility is the necessary interpretation of “consistent.”

Conversely assume $F_{xy}=0$. On $x=0$, solve $\partial_yS=-A_yS$ with $S(0,0)=1$. For each $y$, extend it along $x$ by $\partial_xS=-A_xS$. Linear [ordinary differential equations](../../../../../ordinary-differential-equation.md) with smooth coefficients give global invertible [matrices](../../../../../matrix.md) on these finite coordinate paths. Put $R=D_yS$. Since $D_xS=0$,

$$
D_xR=[D_x,D_y]S+D_yD_xS=F_{xy}S=0,\qquad R(0,y)=0.
$$

Uniqueness of the homogeneous transport equation gives $R=0$. Thus $S$ is a full parallel [bundle frame](../../../../../frame-of-a-vector-bundle.md). This proves the [parallel-frame compatibility criterion](../../../../../parallel-frame-compatibility-criterion.md) without assuming a nonzero vector spans the whole fiber.

Geometrically $A=A_xdx+A_ydy$ is a [gauge connection](../../../../../connection-vector-bundle.md) on the trivial real rank-$n$ [vector bundle](../../../../../vector-bundle.md), and $F_{xy}dx\wedge dy$ is its [gauge curvature](../../../../../gauge-field-strength.md). The displayed nonlinear equation is [flat connection](../../../../../flat-connection.md). Writing $g=S^{-1}$ gives its general solution on $\mathbb R^2$:

$$
\boxed{A_x=g^{-1}\partial_xg,\qquad A_y=g^{-1}\partial_yg,\qquad
 g:\mathbb R^2\to GL(n,\mathbb R).}
$$

Conversely substitution, or the [Maurer-Cartan equation](../../../../../maurer-cartan-equation.md), proves that every such [gauge potential](../../../../../gauge-field.md) is flat. The parallel sections are $v=g^{-1}c$ for constant columns $c$. Multiplying $g$ on the left by a constant [matrix](../../../../../matrix.md) leaves $A$ unchanged. On a nonsimply connected domain a [flat connection](../../../../../flat-connection.md) can have nontrivial [holonomy](../../../../../holonomy.md), so a single-valued global pure-gauge expression needs an extra [holonomy](../../../../../holonomy.md) condition; the specified plane has no such obstruction.

For the [Bogomolny equations](../../../../../bogomolny-equations.md), complexify the auxiliary [vector space](../../../../../vector-space-split.md) and introduce the [spectral parameter](../../../../../spectral-parameter.md) $\lambda$. Let $\Phi$ denote multiplication by the Higgs [matrix](../../../../../matrix.md), while $D_i\Phi$ denotes its adjoint [gauge covariant derivative](../../../../../gauge-covariant-derivative.md). Define the [Lax pair for the Bogomolny equations](../../../../../lax-pair-for-the-bogomolny-equations.md)

$$
\boxed{L_0(\lambda)=D_1+iD_2-\lambda(D_3+i\Phi),\qquad
L_1(\lambda)=D_3-i\Phi+\lambda(D_1-iD_2).}
$$

The auxiliary equations are $L_0(\lambda)\psi=L_1(\lambda)\psi=0$. To check their compatibility, use $[D_i,D_j]=F_{ij}$ and $[D_i,\Phi]=D_i\Phi$. Put

$$
a=F_{12}-D_3\Phi,\quad b=F_{31}-D_2\Phi,\quad c=F_{23}-D_1\Phi.
$$

The constant, linear and quadratic terms in the [matrix commutator](../../../../../commutator.md) are respectively

$$
[L_0,L_1]=-b+ic-2i\lambda a-\lambda^2(b+ic).
$$

Thus vanishing for every $\lambda$ forces $a=0$, $b=0$, $c=0$, and those conditions also make the [matrix commutator](../../../../../commutator.md) zero. They are exactly $\tfrac12\epsilon_{ijk}F_{jk}=D_i\Phi$. No spectral-parameter [derivative](../../../../../derivative.md) is needed. Homogenizing in the two projective coordinates of $\lambda\in\mathbb{CP}^1$ includes the point at infinity.

The dimensional-reduction interpretation is equally explicit. On Euclidean $\mathbb R^4$ with orientation $1234$, take fields independent of $x^4$ and set $A_4=-\Phi$. Then $F_{i4}=-D_i\Phi$. [Anti-self-duality of gauge curvature](../../../../../anti-self-duality-of-gauge-curvature.md) says $F_{12}=-F_{34}$, $F_{23}=-F_{14}$, and $F_{31}=-F_{24}$, which reduce to the same three [Bogomolny equations](../../../../../bogomolny-equations.md). Translation symmetry reduction therefore turns the four-dimensional [ASDYM](../../../../../anti-self-dual-yang-mills-equations.md) zero-curvature system into the parameter-dependent three-dimensional system above.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
