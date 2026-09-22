<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Butcher contractivity theorem](../../../../../../butcher-contractivity-theorem.md) states that an [algebraically stable](../../../../../../algebraic-stability-of-a-runge-kutta-method.md) [Runge-Kutta method](../../../../../../runge-kutta-method.md) is [B-stable](../../../../../../b-stability.md): for a [dissipative vector field](../../../../../../dissipative-vector-field.md) and any positive step for which the stage problems are solved, its step does not increase the distance between two numerical solutions. The required condition on the [dissipative vector field](../../../../../../dissipative-vector-field.md) is

$$
\operatorname{Re}\langle f(t,u)-f(t,v),u-v\rangle\leq0
$$

for all compared states at each common time. The [inner product](../../../../../../inner-product.md) can be real Euclidean or complex Hermitian. The [stage solvability of an implicit Runge-Kutta method](../../../../../../stage-solvability-of-an-implicit-runge-kutta-method.md) is assumed in this comparison, not a conclusion from a distance estimate alone.

Let $d$ be the difference of starting values, $D_i$ the differences of corresponding stages and $F_i$ the differences of their vector-field values. Then

$$
D_i=d+h\sum_ja_{ij}F_j,\qquad
 d_+=d+h\sum_i b_iF_i.
$$

Expanding the squared [norm](../../../../../../norm.md) of the update gives

$$
\|d_+\|^2=\|d\|^2+2h\sum_i b_i\operatorname{Re}\langle d,F_i\rangle
+h^2\sum_{i,j}b_ib_j\operatorname{Re}\langle F_i,F_j\rangle.
$$

Substitute $d=D_i-h\sum_ja_{ij}F_j$ in the linear term. Symmetrizing the double sum proves the [Runge-Kutta contractivity identity](../../../../../../runge-kutta-contractivity-identity.md)

$$
\boxed{\|d_+\|^2=\|d\|^2
+2h\sum_i b_i\operatorname{Re}\langle D_i,F_i\rangle
-h^2\sum_{i,j}m_{ij}\operatorname{Re}\langle F_i,F_j\rangle.}
$$

Each [inner product](../../../../../../inner-product.md) in the first sum is nonpositive by the defining inequality for a [dissipative vector field](../../../../../../dissipative-vector-field.md), and its weight is nonnegative. The final [quadratic form](../../../../../../quadratic-form.md) is nonnegative: resolve the [vectors](../../../../../../vector.md) $F_i$ into components and apply [positive semidefiniteness](../../../../../../positive-semidefinite-matrix.md) of $M$ to each component [vector](../../../../../../vector.md). Hence $\boxed{\|d_+\|\leq\|d\|}$, which is exactly [B-stability](../../../../../../b-stability.md). No [linearization](../../../../../../linearization.md) of the [vector field](../../../../../../vector-field.md) has been used.

For the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md) $y'=\lambda y$ with $\operatorname{Re}\lambda\leq0$, this also bounds the amplification factor by one wherever the stages are well defined. With strictly positive weights, no stage pole can occur in the open left half-plane. Indeed, if $(I-zA)v=0$ for nonzero $v$, then

$$
v^*Mv=2\operatorname{Re}(1/z)v^*Bv-|b^Tv|^2<0
$$

when $\operatorname{Re}z<0$, contradicting $M\succeq0$. This proves the usual [A-stability](../../../../../../a-stability.md) corollary for the scalar [stability function](../../../../../../stability-function.md); boundedness from the open half-plane makes any boundary pole in that [rational function](../../../../../../rational-function.md) removable. Zero-weight redundant stages require their own solvability treatment. The nonlinear [B-stability](../../../../../../b-stability.md) statement is stronger than [A-stability](../../../../../../a-stability.md), and the two notions should not be conflated.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
