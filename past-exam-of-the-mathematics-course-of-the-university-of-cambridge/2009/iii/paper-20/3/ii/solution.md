<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the unknot the three-manifolds are **$S^3$, $U_0=S^1\times S^2$, and $U_n=L_n$**, where $L_n$ denotes positive $n$-surgery with its surgery orientation. This fixes the orientation independently of competing conventions for the name $L(n,1)$.

Use the grading convention $\operatorname{gr}\Theta^+_{S^3}=0$ and $\operatorname{gr}\Theta^-_{S^3}=-2$. Let $R=\mathbb Z[U]$ and $\widehat R=\mathbb Z[[U]]$. The ordinary minus groups are

$$
\boxed{\begin{aligned}
HF^-(S^3)&=R\langle\Theta^-\rangle,&\operatorname{gr}\Theta^-&=-2,\\
HF^-(S^1\times S^2,\mathfrak s_0)&=R\langle x_+\rangle\oplus R\langle x_-\rangle,&(\operatorname{gr}x_+,\operatorname{gr}x_-)&=(-3/2,-5/2),\\
HF^-(S^1\times S^2,\mathfrak s_i)&=R/(1-U^{|i|})\quad(i\ne0),\\
HF^-(L_n,\mathfrak t_k)&=R\langle y_k\rangle,&\operatorname{gr}y_k&=d_k-2,
\end{aligned}}
$$

where $0\le k<n$ and

$$
\boxed{d_k=\frac{(2k-n)^2-n}{4n}.}
$$

The lens-space absolute grading can be calculated from the standard torus surgery triple. For $0\le k<n$, the reverse trace structure with evaluation $2k-n$ has a small embedded holomorphic triangle with basepoint multiplicity zero and signed count $\pm1$, taking $y_k$ to $\Theta^-$. Its degree shift is $\Delta_k=(1-(2k-n)^2/n)/4$. Thus $(d_k-2)+\Delta_k=-2$, which gives the boxed formula for $d_k$. Additional triangles wind around the surgery region and give the higher powers of $U$ calculated below.

Their infinity groups are obtained by inverting $U$: one Laurent tower for $S^3$ and each lens-space structure, two for the torsion structure on $S^1\times S^2$, and $\mathbb Z[U,U^{-1}]/(1-U^{|i|})$ in its non-torsion structures. Their plus groups are respectively $\mathcal T^+_0$, $\mathcal T^+_{1/2}\oplus\mathcal T^+_{-1/2}$, and $\mathcal T^+_{d_k}$. The hat groups are $\mathbb Z$ in degree zero, $\mathbb Z$ in each degree $\pm1/2$, and $\mathbb Z$ in degree $d_k$. These follow directly by straightening the standard genus-one [Heegaard diagrams](../../../../../../heegaard-diagram.md): the [lens space](../../../../../../lens-space.md) has one generator in each structure and no [chain differential](../../../../../../boundary-operator.md), while the two bigons in the torsion $S^1\times S^2$ diagram cancel with coherent signs. The [sphere](../../../../../../sphere.md) adjunction condition eliminates its non-torsion plus and hat groups, but not its ordinary minus group. The [Non-torsion Heegaard Floer homology of the sphere-circle product](../../../../../../non-torsion-heegaard-floer-homology-of-the-sphere-circle-product.md) calculation comes from a two-generator [chain complex](../../../../../../chain-complex.md) with [chain differential](../../../../../../boundary-operator.md) $1-U^{|i|}$; its cokernel is the displayed quotient. For the triangle, complete the free minus towers by replacing $R$ with $\widehat R$. The non-torsion summands disappear after completion, because $1-U^{|i|}$ has an inverse $1+U^{|i|}+U^{2|i|}+\cdots$ in $\widehat R$.

For $k=0$, choose signs so that the exact triangle becomes

$$
\boxed{\widehat R\xrightarrow{\ 1\mapsto x_-\ }\widehat R x_+\oplus\widehat R x_-\xrightarrow{\ x_+\mapsto y_0,\ x_-\mapsto0\ }\widehat R y_0\xrightarrow{\ 0\ }\widehat R.}
$$

The zero-surgery trace has $\chi=1$, $\sigma=0$, and $c_1^2=0$ in the torsion structure; hence its absolute degree shift is $-1/2$, taking $\Theta^-$ to $x_-$. The auxiliary-generator map takes $x_+$ to $y_0$, so its effective grading shift is

$$
(d_0-2)-(-3/2)=\boxed{(n-3)/4}.
$$

For the underlying [cobordism](../../../../../../cobordism.md) $Z_n$ in its torsion structure, $c_1^2=0$, $\chi=1$, $\sigma=0$, and its actual [cobordism](../../../../../../cobordism.md) shift is $-1/2$. Tensoring with the canonical lens generator adds $d_0=(n-1)/4$ under the connected-sum grading convention, explaining the effective shift. For $n=1$ the auxiliary [lens space](../../../../../../lens-space.md) is $S^3$, and this is simply the other degree-$-1/2$ surgery trace map.

The reverse trace components are explicit in every $k$. For $j=k+n\ell$, put $m_j=2j-n$. Its [intersection form](../../../../../../intersection-form.md) is $(-n)$, so

$$
\Delta_j=\frac{1-m_j^2/n}{4},\qquad
F^-_{V_n,\mathfrak r_j}(y_k)=\pm U^{r_\ell}\Theta^-,\qquad
r_\ell=\frac{m_j^2-(2k-n)^2}{8n}=\frac{n\ell(\ell-1)}2+k\ell.
$$

Indeed $c_1^2=-m_j^2/n$, $\chi=1$, $\sigma=-1$, and matching source and target degrees gives precisely the displayed exponent. The exponent is nonnegative, and the coefficient is a unit: the infinity trace map is an isomorphism, and restriction to the free minus towers leaves the unique grading-compatible monomial.

With a compatible choice of [Coherent orientations in Heegaard Floer homology](../../../../../../coherent-orientations-in-heegaard-floer-homology.md), the sum $C_k$ is multiplication by

$$
P_k(U)=\sum_{\ell\in\mathbb Z}(-1)^\ell U^{n\ell(\ell-1)/2+k\ell}.
$$

For $k=0$, pair $\ell$ with $1-\ell$: their exponents agree and their signs are opposite, so $P_0=0$, in agreement with the first triangle. For $0<k<n$ the term $\ell=0$ is the unique constant term, and every other exponent is positive. Thus $P_k=1+U(\cdots)$ is a unit in $\widehat R$. The zero-surgery summand for such a $k$ vanishes, and the exact triangle is

$$
\boxed{\widehat R\longrightarrow0\longrightarrow\widehat R y_k\xrightarrow{\ P_k(U)\ }\widehat R,\qquad0<k<n.}
$$

It is isomorphic, as an ungraded completed-module triangle, to one with the final map the identity. The sum generally has no single [absolute Heegaard Floer grading](../../../../../../absolute-grading-in-heegaard-floer-homology.md) shift; **each individual trace component has shift $\Delta_j$**. This distinction and the power series explain why replacing the completed triangle by a polynomial-module triangle is not innocuous.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
