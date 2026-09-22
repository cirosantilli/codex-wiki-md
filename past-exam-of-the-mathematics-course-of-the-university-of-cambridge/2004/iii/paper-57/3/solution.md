<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Keep the unit-normal sign explicit: $n^an_a=\varepsilon\in\{+1,-1\}$. Since the hypersurface is spacelike its normal is timelike. Construct

$$
n_a=\pm\frac{\nabla_af}{\sqrt{|g^{bc}\nabla_bf\nabla_cf|}},\qquad h_{ab}=g_{ab}-\varepsilon n_an_b,\qquad h_a{}^b=\delta_a{}^b-\varepsilon n_an^b.
$$

Choose the sign of n for the desired time orientation. The pullback of h is the nondegenerate [induced metric](../../../../../induced-metric.md). The [second fundamental form](../../../../../second-fundamental-form-split.md) is

$$
\boxed{K_{ab}=h_a{}^ch_b{}^d\nabla_cn_d.}
$$

Its sign reverses when n reverses. It is tangential in both indices and symmetric: the antisymmetric part of the derivative of a normalized gradient vanishes after both tangential projections. Equivalently it is the projected Hessian of f divided by the normalizing factor. This is the normal-change definition of [extrinsic curvature](../../../../../extrinsic-curvature.md).

For tangent vector fields X,Y, let D be the induced [Levi-Civita connection](../../../../../levi-civita-connection.md). Orthogonality to n gives the derivative decomposition

$$
\nabla_XY=D_XY-\varepsilon K(X,Y)n,\qquad g(\nabla_Xn,Y)=K(X,Y).
$$

Use the curvature convention of the preceding solution, $R(X,Y)Z=[\nabla_X,\nabla_Y]Z-\nabla_{[X,Y]}Z$. Substitute the decomposition twice and take its tangential component. Terms differentiated normally cancel, while the two normal components contribute the quadratic shape terms:

$$
P R^{(4)}(X,Y)Z=R^{(3)}(X,Y)Z-\varepsilon\{K(Y,Z)\nabla_Xn-K(X,Z)\nabla_Yn\}.
$$

Lowering the first curvature index gives the [Gauss equation for a nonnull hypersurface](../../../../../gauss-equation-for-a-nonnull-hypersurface.md)

$$
\boxed{{}^{(3)}R_{abcd}=h_a{}^eh_b{}^fh_c{}^gh_d{}^k{}^{(4)}R_{efgk}+\varepsilon(K_{ac}K_{bd}-K_{ad}K_{bc}).}
$$

All four displayed indices on the left are tangential.

Contract with $h^{ac}h^{bd}$ and use $h^{ab}=g^{ab}-\varepsilon n^an^b$ for tangential contractions. The double-normal term vanishes by curvature antisymmetry and each mixed contraction is ambient [Ricci curvature](../../../../../ricci-curvature.md). With $K=h^{ab}K_{ab}$ this gives

$$
\boxed{{}^{(3)}R={}^{(4)}R-2\varepsilon\,{}^{(4)}R_{ab}n^an^b+\varepsilon(K^2-K_{ab}K^{ab}).}
$$

This also records which metric and curvature conventions enter the sign.

In vacuum without a cosmological constant, the ambient [Ricci tensor](../../../../../ricci-tensor.md) and scalar vanish. A [totally umbilic hypersurface](../../../../../totally-umbilic-hypersurface.md) has $K_{ab}=\lambda h_{ab}$, so $K=3\lambda$ and $K_{ab}K^{ab}=3\lambda^2$. Therefore the [scalar curvature of an umbilic vacuum hypersurface](../../../../../scalar-curvature-of-an-umbilic-vacuum-hypersurface.md) is $6\varepsilon\lambda^2$.

To express the requested nonnegative version, take Lorentz signature $(+---)$, so the timelike [unit normal](../../../../../unit-normal.md) has $\varepsilon=+1$ and h is the induced negative-definite spatial metric. Then

$$
\boxed{{}^{(3)}R=6\lambda^2=\frac23K^2\geq0.}
$$

If instead one uses signature $(-+++)$ and its positive-definite spatial metric with the same curvature-slot convention, the scalar is $-6\lambda^2$. Replacing h by $-h$ reverses its scalar curvature. Thus the printed inequality has a signature/induced-metric convention built into it; the general formula above makes that choice explicit rather than losing the sign. The metric in the separate final question explicitly uses the mostly-plus signature.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
