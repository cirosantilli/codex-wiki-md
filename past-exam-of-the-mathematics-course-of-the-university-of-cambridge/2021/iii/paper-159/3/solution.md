<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [irregularity of an algebraic surface](../../../../../irregularity-of-an-algebraic-surface.md) and the [geometric genus of an algebraic surface](../../../../../geometric-genus-of-an-algebraic-surface.md) are respectively

$$
q(X)=h^1(X,\mathcal O_X)=h^0(X,\Omega_X^1),
\qquad
p_g(X)=h^0(X,K_X)=h^2(X,\mathcal O_X).
$$

If $\pi:X'\to X$ is the blowup at a point with [exceptional divisor](../../../../../exceptional-divisor.md) $E$, then

$$
K_{X'}=\pi^*K_X+E.
$$

A holomorphic two-form on $X$ pulls back to one on $X'$. Conversely, a holomorphic two-form on $X'$ descends across $E$: locally it is a form on the punctured smooth surface $X\setminus\{p\}$, and its coefficients extend over the codimension-two point $p$. Equivalently, $\pi_*K_{X'}=K_X$. Pullback is therefore an isomorphism

$$
H^0(X,K_X)\cong H^0(X',K_{X'}),
$$

which proves the [birational invariance of the geometric genus of a surface](../../../../../birational-invariance-of-the-geometric-genus-of-a-surface.md) in this case.

Let $X=C\times D$, where both smooth projective curves have positive genus. The [Künneth theorem](../../../../../kunneth-theorem.md) gives the [irregularity of a product of curves](../../../../../irregularity-of-a-product-of-curves.md)

$$
q(X)=g(C)+g(D)>0.
$$

If a surface is a hypersurface in projective space, dimension forces it to be a smooth hypersurface $Y\subseteq\mathbb P^3$. From

$$
0\longrightarrow\mathcal O_{\mathbb P^3}(-d)
\longrightarrow\mathcal O_{\mathbb P^3}
\longrightarrow\mathcal O_Y
\longrightarrow0
$$

and the intermediate cohomology vanishing for line bundles on projective space, one obtains $H^1(Y,\mathcal O_Y)=0$. Thus every such hypersurface has irregularity zero, whereas $X$ has positive irregularity. Hence $C\times D$ is not isomorphic to a hypersurface. This is the [product of positive-genus curves is not a projective hypersurface](../../../../../product-of-positive-genus-curves-is-not-a-projective-hypersurface.md) obstruction.

The [Albanese variety](../../../../../albanese-variety.md) $\operatorname{Alb}(X)$ is the universal [abelian variety](../../../../../abelian-variety-split.md) receiving a pointed morphism from $X$, and

$$
\dim\operatorname{Alb}(X)=q(X).
$$

Let the smooth image curve of the Albanese morphism be $C$ of genus $g$. Pullback of holomorphic one-forms along the dominant map $X\to C$ is injective, giving $g\leq q(X)$. On the other hand, the universal property of the Jacobian extends $C\to\operatorname{Alb}(X)$ to a homomorphism

$$
\operatorname{Jac}(C)\longrightarrow\operatorname{Alb}(X).
$$

The Albanese image generates the entire Albanese variety, so this homomorphism is surjective and $q(X)\leq\dim\operatorname{Jac}(C)=g$. Therefore the [Irregularity from a smooth Albanese curve image](../../../../../irregularity-from-a-smooth-albanese-curve-image.md) is

$$
\boxed{q(X)=g}.
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 159](../../paper-159-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
