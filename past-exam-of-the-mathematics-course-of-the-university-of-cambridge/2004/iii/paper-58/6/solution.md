<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Let $\eta_{ab}=g(e_a,e_b)$ be the constant diagonal metric matrix in a local [pseudo-orthonormal frame](../../../../../pseudo-orthonormal-frame.md), and define $\theta_{ab}=\eta_{ac}\theta^c{}_b$. The [metric compatibility](../../../../../metric-compatibility.md) of the [Levi-Civita connection](../../../../../levi-civita-connection.md) gives

$$
0=d\eta_{ab}=g(\nabla e_a,e_b)+g(e_a,\nabla e_b)=\theta_{ba}+\theta_{ab}.
$$

Thus **the lowered connection matrix is antisymmetric**, including in indefinite signature. Ordinary matrix antisymmetry of $\theta^a{}_b$ itself is not the corresponding assertion in indefinite signature.

Let $\omega^a$ be the dual [coframe](../../../../../coframe.md), and write a vector field as $Y=e_b\omega^b(Y)$. Then

$$
\omega^a(\nabla_XY)=X\big(\omega^a(Y)\big)+\theta^a{}_b(X)\omega^b(Y).
$$

Subtract the same expression with $X,Y$ exchanged and subtract $\omega^a([X,Y])$. By the definition of the [exterior derivative](../../../../../exterior-derivative.md), this gives the components of the [torsion tensor](../../../../../torsion-tensor.md):

$$
\omega^a\big(\nabla_XY-\nabla_YX-[X,Y]\big)=d\omega^a(X,Y)+(\theta^a{}_b\wedge\omega^b)(X,Y).
$$

The [Levi-Civita connection](../../../../../levi-civita-connection.md) is [torsion-free](../../../../../torsion-free-connection.md), so [Cartan's first structure equation](../../../../../cartan-s-first-structure-equation.md) is

$$
\boxed{d\omega^a+\theta^a{}_b\wedge\omega^b=0.}
$$

Use $R(X,Y)=\nabla_X\nabla_Y-\nabla_Y\nabla_X-\nabla_{[X,Y]}$ and define its matrix of [curvature two-forms](../../../../../curvature-2-form.md) by $R(X,Y)e_b=e_aR^a{}_b(X,Y)$. Applying two [covariant derivatives](../../../../../covariant-derivative.md) to $e_b$ yields

$$
R^a{}_b(X,Y)=X\big(\theta^a{}_b(Y)\big)-Y\big(\theta^a{}_b(X)\big)-\theta^a{}_b([X,Y])
+\theta^a{}_c(X)\theta^c{}_b(Y)-\theta^a{}_c(Y)\theta^c{}_b(X).
$$

The first three terms are $d\theta^a{}_b(X,Y)$ and the last two are $(\theta^a{}_c\wedge\theta^c{}_b)(X,Y)$. Therefore [Cartan's second structure equation](../../../../../cartan-s-second-structure-equation.md) is

$$
\boxed{R^a{}_b=d\theta^a{}_b+\theta^a{}_c\wedge\theta^c{}_b.}
$$

The associated [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) components satisfy $R^a{}_b=\tfrac12R^a{}_{bcd}\omega^c\wedge\omega^d$ with this convention.

For a position-dependent change of [pseudo-orthonormal frame](../../../../../pseudo-orthonormal-frame.md), write the frame row as $E'=E\Lambda$, with $\Lambda^T\eta\Lambda=\eta$. The dual [coframe](../../../../../coframe.md) obeys $\omega'=\Lambda^{-1}\omega$. Applying the [Leibniz rule](../../../../../leibniz-rule.md) to $\nabla(E\Lambda)$ gives

$$
\theta'=\Lambda^{-1}\theta\Lambda+\Lambda^{-1}d\Lambda.
$$

The [connection one-form](../../../../../connection-one-form.md) has an inhomogeneous term because differentiating the moving basis produces $d\Lambda$. The [curvature two-form](../../../../../curvature-2-form.md) instead transforms homogeneously. Indeed, [curvature](../../../../../curvature.md) is tensorial in the vector to which it is applied, so $R(X,Y)(E\Lambda)=(R(X,Y)E)\Lambda=E'\Lambda^{-1}R(X,Y)\Lambda$. Consequently

$$
\boxed{R'=\Lambda^{-1}R\Lambda,\qquad R'^a{}_b=(\Lambda^{-1})^a{}_cR^c{}_d\Lambda^d{}_b.}
$$

Equivalently, substituting the transformed connection into $d\theta'+\theta'\wedge\theta'$ and using $d\Lambda^{-1}=-\Lambda^{-1}(d\Lambda)\Lambda^{-1}$ cancels all derivative terms and gives the same result. This transformation law holds for a general invertible frame change as well; the orthogonality condition ensures both frames remain pseudo-orthonormal.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
