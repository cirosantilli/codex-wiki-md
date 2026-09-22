<h1 id="24g/solution">Solution</h1>

↑ **Parent:** [24G](../24g.md)

Two irreducible [varieties](../../../../../algebraic-variety.md) $X$ and $Y$ are [birational](../../../../../birational-variety.md) if they contain nonempty [Zariski-open subsets](../../../../../zariski-open-set.md) $U\subseteq X$ and $V\subseteq Y$ that are isomorphic. Equivalently, their [function fields](../../../../../function-field-of-an-algebraic-variety.md) are isomorphic:

$$
k(X)\cong k(Y).
$$

For an irreducible variety,

$$
\dim X=\operatorname{trdeg}_k k(X).
$$

An isomorphism of function fields preserves transcendence degree, so $\dim X=\dim Y$. This is the [dimension from the function field](../../../../../dimension-from-the-function-field.md).

Now let $K/\mathbb C$ be a finitely generated field extension. Choose field generators $a_1,\ldots,a_m$ and set

$$
A=\mathbb C[a_1,\ldots,a_m]\subseteq K.
$$

Then $A$ is a finitely generated integral $\mathbb C$-algebra and $\operatorname{Frac}(A)=K$. The affine irreducible variety

$$
X_0=\operatorname{Spec}A
$$

has function field $K$. Embed $X_0$ as a closed affine subvariety of some affine space $\mathbb A^N$, identify that affine space with the standard open chart of [projective space](../../../../../projective-space-split.md) $\mathbb P^N$, and take the projective closure $X$ of $X_0$. The closure of an [irreducible topological space](../../../../../irreducible-topological-space.md) is irreducible, and $X_0$ is dense and open in $X$. Thus $X$ is a [projective variety](../../../../../projective-variety.md) and

$$
k(X)=k(X_0)=K.
$$

This constructs the [projective model of a finitely generated field](../../../../../projective-model-of-a-finitely-generated-field.md).

For the curve

$$
X=V\bigl(y^2-x(x-1)^2\bigr),
$$

put

$$
t=\frac y{x-1}.
$$

In its function field, the defining equation gives

$$
t^2=x,
\qquad
y=t(x-1)=t(t^2-1).
$$

Hence $\mathbb C(X)=\mathbb C(t)$, so $X$ is rational. Equivalently, this is the [normalization of y squared equals x times x minus one squared](../../../../../normalization-of-y-squared-equals-x-times-x-minus-one-squared.md), whose smooth projective normalization is $\mathbb P^1$ and has [geometric genus](../../../../../geometric-genus.md) zero.

A [smooth projective curve](../../../../../smooth-projective-curve.md) in the [projective plane](../../../../../projective-plane.md) of degree $d$ has, by the [genus of a smooth plane curve](../../../../../genus-of-a-smooth-plane-curve.md) formula,

$$
g=\frac{(d-1)(d-2)}2.
$$

Its genus can be zero only for $d=1$ or $d=2$. Conversely, a projective line and every smooth conic over $\mathbb C$ are rational, so each is birational to $X$. Therefore the required degrees are exactly

$$
\boxed{d=1\text{ or }d=2}.
$$

Finally, in $\mathbb A^3_{x,y,z}$ take

$$
S=V(F),
\qquad
F(x,y,z)=y^2-x(x-1)^2.
$$

The polynomial $F$ is irreducible: as a quadratic in $y$, it could factor only if $x(x-1)^2$ were a square polynomial, which it is not. Thus $S$ is an irreducible [affine hypersurface](../../../../../affine-hypersurface.md) of dimension two. Its function field is

$$
\mathbb C(S)=\mathbb C(t,z),
\qquad
x=t^2,
\qquad
y=t(t^2-1),
$$

so $S$ is birational to $\mathbb A^2$.

The partial derivatives are

$$
F_x=-(x-1)(3x-1),
\qquad F_y=2y,
\qquad F_z=0.
$$

Solving $F=F_x=F_y=0$ gives $x=1$, $y=0$, with $z$ arbitrary. By the [Jacobian criterion](../../../../../zariski-tangent-space.md),

$$
\operatorname{Sing}(S)=\{(1,0,z):z\in\mathbb C\}\cong\mathbb A^1.
$$

This is an irreducible subvariety of dimension one, giving the requested [singular cylinder over a nodal curve](../../../../../singular-cylinder-over-a-nodal-curve.md).

## ↑ Ancestors (10)

1. [24G](../24g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
