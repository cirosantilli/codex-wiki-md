<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

First fix distinct $q_1,\ldots,q_k$ and let $Q=q_1+\cdots+q_k$. A [negative-degree divisor has no sections](../../../../negative-degree-divisor-has-no-sections.md): if $0\ne f\in\mathcal L(D)$, then $(f)+D$ is an [effective divisor](../../../../effective-cartier-divisor.md) of degree $\deg D$, since a [principal divisor](../../../../principal-divisor-on-an-algebraic-curve.md) has degree zero, so $\deg D$ cannot be negative. As $\deg K=0$ and $\deg(K-Q)=-k<0$, the [Riemann-Roch theorem](../../../../riemann-roch-theorem.md) therefore gives

$$
\boxed{\ell(Q)=\deg Q+1-g+\ell(K-Q)=k.}
$$

Now choose distinct $p_1,\ldots,p_k$ outside the support of $Q$, and put $P=p_1+\cdots+p_k$. A function with the required zeros and [poles](../../../../pole.md) must be a nonzero element of $\mathcal L(Q-P)$. Conversely, if $0\ne f\in\mathcal L(Q-P)$, then $(f)+Q-P$ is an [effective divisor](../../../../effective-cartier-divisor.md) of degree zero, hence is zero. It follows that $(f)=P-Q$, giving precisely the required simple zeros and simple [poles](../../../../pole.md), with no others. Thus the existence question is exactly whether $\mathcal L(Q-P)\ne0$.

Take a [basis](../../../../basis.md) $f_1,\ldots,f_k$ of the [Riemann-Roch space](../../../../riemann-roch-space.md) $\mathcal L(Q)$. Evaluation at the $p_i$ defines the [linear map](../../../../linear-map.md)

$$
E_P:\mathcal L(Q)\longrightarrow\mathbb C^k,
\qquad f\longmapsto(f(p_1),\ldots,f(p_k)),
$$

whose [kernel](../../../../kernel-of-a-linear-map-split.md) is $\mathcal L(Q-P)$. The [evaluation criterion for a prescribed principal divisor](../../../../evaluation-criterion-for-a-prescribed-principal-divisor.md) becomes

$$
\mathcal L(Q-P)\ne0
\iff
\Delta(p_1,\ldots,p_k):=\det(f_j(p_i))_{1\leq i,j\leq k}=0.
$$

The crucial point is that this [determinant](../../../../determinant.md) does not vanish identically; a count of unknowns and equations alone would not prove this.

To verify it, begin with $V_0=\mathcal L(Q)$, of [dimension](../../../../dimension-vector-space.md) $k$. Whenever $V_{j-1}\ne0$, choose a nonzero $f\in V_{j-1}$. Its zeros are finite. Choose $p_j$ outside those zeros, the support of $Q$ and the previously chosen points. Evaluation at $p_j$ is then a nonzero linear functional on $V_{j-1}$, so

$$
V_j=\{h\in V_{j-1}:h(p_j)=0\},
\qquad \dim V_j=\dim V_{j-1}-1.
$$

After $k$ steps, $V_k=0$. Thus there exists a tuple of distinct points with $\Delta\ne0$.

The entries of this [determinant](../../../../determinant.md) vary [holomorphically](../../../../holomorphic-function-split.md) away from the $q_i$, and are [rational functions](../../../../rational-function.md) on the nonsingular [projective curve](../../../../projective-curve.md). Its vanishing is therefore a proper closed exceptional locus on this configuration space; its complement is open and dense in the [Zariski topology](../../../../zariski-topology.md). For a generic choice of the $p_i$, $E_P$ is invertible and

$$
\boxed{\ell(Q-P)=0,\quad\text{so no function with the prescribed zeros and poles exists}.}
$$

This holds for every fixed tuple of distinct $q_i$, which proves the assertion for generic choices of both sets of points. At $k=1$, it is especially transparent: $\mathcal L(q_1)=\mathbb C$, so no nonzero member can vanish at a distinct $p_1$.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the algebraic curves course of the University of Oxford](../../../split.md)
5. [Algebraic curves course of the University of Oxford](../../../../algebraic-curves-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
