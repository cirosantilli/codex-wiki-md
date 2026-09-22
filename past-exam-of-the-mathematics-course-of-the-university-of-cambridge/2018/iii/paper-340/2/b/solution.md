<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At zero, the partial products are $m(0)^n$. Their assumed convergence and $|m(0)|=1$ force $m(0)=1$ and $\Theta(0)=1$. Uniform convergence on compact sets makes $\Theta$ continuous. The identity with $k=0$ gives $\Theta\in L^2$ with squared norm $2\pi$. Define $\varphi$ by the inverse [Fourier transform](../../../../../../fourier-transform.md) in $L^2$. The [Plancherel theorem](../../../../../../plancherel-theorem.md) and the other given integral identities give

$$
\langle\varphi(\cdot-k),\varphi(\cdot-l)\rangle=\delta_{kl}.
$$

Define $V_j$ as the closed span of $\varphi_{j,k}(x)=2^{j/2}\varphi(2^jx-k)$. These functions form an [orthonormal basis](../../../../../../orthonormal-basis.md) of $V_j$, and dyadic dilation gives the scale axiom. Shifting the infinite product gives

$$
\Theta(2\xi)=m(\xi)\Theta(\xi),
$$

so the finite Fourier series of $m$ gives a [scaling refinement equation](../../../../../../scaling-refinement-equation.md) and $V_j\subset V_{j+1}$. The coarse-scale projection argument of part 1(b) proves the trivial-intersection axiom.

For density, take a function $f$ with bounded Fourier support. The [MRA projection Fourier identity](../../../../../../mra-projection-fourier-identity.md) gives, for large $j$,

$$
\|P_jf\|_2^2=\frac1{2\pi}\int|\widehat f(\xi)|^2|\Theta(2^{-j}\xi)|^2\,d\xi\longrightarrow\|f\|_2^2.
$$

Uniform convergence of $\Theta(2^{-j}\xi)$ to one on that support proves the limit. Since $P_j$ is an [orthogonal projection](../../../../../../orthogonal-projection.md), $\|f-P_jf\|_2^2=\|f\|_2^2-\|P_jf\|_2^2\to0$. Such functions are dense in $L^2$, giving

$$
\boxed{\overline{\bigcup_jV_j}=L^2(\mathbb R).}
$$

Thus all the [multiresolution analysis](../../../../../../multiresolution-analysis.md) axioms hold. Under the strong convergence and orthogonality assumptions supplied here, the additional nonvanishing condition is not needed in this last verification; it is useful when establishing those assumptions from a filter.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
