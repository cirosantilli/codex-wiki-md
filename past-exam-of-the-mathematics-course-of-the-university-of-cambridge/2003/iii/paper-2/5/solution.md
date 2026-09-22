<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The base ring must be specified in the algebraic definition. For a commutative $k$-algebra $R$, work in $\operatorname{End}_k(R)$ and let $m_f$ mean multiplication by $f\in R$. Set $D_k^{-1}(R)=0$ and define recursively

$$
D_k^i(R)=\{P\in\operatorname{End}_k(R):[P,m_f]\in D_k^{i-1}(R)\text{ for every }f\in R\}.
$$

These are the operators of order at most $i$. The order of a nonzero [differential operator relative to a base ring](../../../../../differential-operator-relative-to-a-base-ring.md) is the least $i$ for which it belongs to $D_k^i(R)$; the zero operator can be assigned order $-\infty$. An operator of order zero commutes with all multiplications and is itself multiplication by $P(1)$, so $D_k^0(R)=R$. The union $D_k(R)=\bigcup_{i\ge0}D_k^i(R)$ is the ring of finite-order operators, with composition as multiplication. The identity

$$
[PQ,m_f]=P[Q,m_f]+[P,m_f]Q
$$

and induction on the sum of orders give $D_k^pD_k^q\subseteq D_k^{p+q}$. Sums have order at most the maximum of their orders, proving that this union is a ring.

For an arbitrary commutative ring, the absolute version uses $k=\mathbb Z$, so the ambient endomorphisms are additive. **For the polynomial ring in this question, the intended Weyl-algebra identification is the relative one with $k=\mathbb C$.** Absolute operators would also include nonzero derivations of the coefficient field $\mathbb C$: a derivation on a rational function field in a transcendence basis over $\mathbb Q$ extends to its algebraic closure in characteristic zero, and hence to $\mathbb C$. Extending it coefficientwise to $\mathbb C[x]$ gives an order-one additive operator which is not complex-linear. Such an operator cannot belong to the complex [Weyl algebra](../../../../../weyl-algebra.md). This explains why the linearity convention matters.

Now take $R=\mathbb C[x_1,\ldots,x_n]$. Coordinate multiplication has order zero, and each partial derivative $\partial_i$ has order one because $[\partial_i,m_f]=m_{\partial_i f}$. They satisfy the defining [Weyl algebra](../../../../../weyl-algebra.md) relations, giving an algebra homomorphism $A_n\to D_\mathbb C(R)$. Reordering spans $A_n$ by $x^\alpha\partial^\beta$. If an ordered expression acted as zero, commutation with the coordinates according to a maximal derivative multiindex would give multiplication by $\beta!f_\beta(x)=0$; removing the top coefficients successively proves that every coefficient is zero. Thus the homomorphism is injective, as in the [ordered monomial basis of a Weyl algebra](../../../../../ordered-monomial-basis-of-a-weyl-algebra.md) proof.

For surjectivity, let $P$ have order at most $m$, and put $\delta_iP=[P,m_{x_i}]$. The operations $\delta_i$ commute, since the coordinate multiplications commute. A product of more than $m$ of them kills $P$. Define polynomial coefficients

$$
a_\beta(x)=\frac{1}{\beta!}(\delta^\beta P)(1),\qquad |\beta|\le m.
$$

Commuting $P$ through $m_{x^\alpha}$ repeatedly gives the finite identity

$$
P(x^\alpha)=\sum_{\beta\le\alpha}\binom{\alpha}{\beta}
 x^{\alpha-\beta}(\delta^\beta P)(1).
$$

It follows by induction on $|\alpha|$ from $Pm_{x_i}=m_{x_i}P+\delta_iP$ and Pascal's identity. Terms with $|\beta|>m$ vanish. Since

$$
\partial^\beta x^\alpha=\beta!\binom{\alpha}{\beta}x^{\alpha-\beta}
$$

for $\beta\le\alpha$, we obtain $P(x^\alpha)=\sum_{|\beta|\le m}a_\beta(x)\partial^\beta(x^\alpha)$. The monomials are a complex basis of $R$, so complex linearity yields equality of the operators on all of $R$. Hence

$$
\boxed{D_\mathbb C(\mathbb C[x_1,\ldots,x_n])=A_n(\mathbb C).}
$$

For a nonzero ordered expression $\sum_\beta a_\beta(x)\partial^\beta$, its order is exactly $\max_{a_\beta\ne0}|\beta|$. The upper bound follows from composition; the lower bound follows by taking that many coordinate commutators to extract a nonzero multiplication operator. This describes the [order filtration of a Weyl algebra](../../../../../order-filtration-of-a-weyl-algebra.md):

$$
D^m(R)=\bigoplus_{|\beta|\le m}R\partial^\beta.
$$

The [associated graded ring](../../../../../associated-graded-ring.md) is therefore

$$
\boxed{\operatorname{gr}_D A_n\cong
\mathbb C[x_1,\ldots,x_n,\xi_1,\ldots,\xi_n],\qquad
\deg x_i=0,\quad\deg\xi_i=1.}
$$

The symbol of $\partial_i$ is $\xi_i$. In a product of ordered operators, moving derivatives past coefficients introduces terms of lower differential order. Thus top-order symbols multiply as ordinary polynomials, and the ordered basis proves there are no further relations. In particular $[D^p,D^q]\subseteq D^{p+q-1}$, with $D^{-1}=0$: the top-order symbols of the two products agree and cancel. Unlike the [Bernstein filtration](../../../../../bernstein-filtration.md), the order filtration's degree-zero part is the entire polynomial ring and its pieces are infinite-dimensional over $\mathbb C$.

Form the [Rees ring of a filtered algebra](../../../../../rees-ring-of-a-filtered-algebra.md)

$$
\mathcal A=\bigoplus_{m\ge0}D^m(R)h^m\subseteq A_n[h].
$$

The central element $h$ is a non-zero-divisor. This ring is generated by $h$, the $x_i$, and $y_i=h\partial_i$, with

$$
[y_i,x_j]=\delta_{ij}h,\qquad [x_i,x_j]=[y_i,y_j]=0.
$$

Its quotient modulo $h$ is the [associated graded ring](../../../../../associated-graded-ring.md) just computed. Explicitly the degree-$m$ component of $h\mathcal A$ is $D^{m-1}h^m$, so the degree-$m$ quotient is $D^m/D^{m-1}$. The quotient modulo $h-1$ recovers $A_n$.

Since $\mathcal A/h\mathcal A$ is commutative, any two lifts $F,G\in\mathcal A$ of symbols have $[F,G]\in h\mathcal A$. Define

$$
\{\overline F,\overline G\}=\frac{[F,G]}h\pmod{h\mathcal A}.
$$

Division by $h$ is unique because $h$ is a non-zero-divisor. If $F$ is replaced by $F+hU$, the quotient changes by $[U,G]$, which is zero modulo $h$; changing $G$ works the same way. Thus the bracket is well defined. Antisymmetry and bilinearity follow from the [commutator](../../../../../commutator.md). The identity $[F,GH]=[F,G]H+G[F,H]$ proves the [Leibniz rule](../../../../../leibniz-rule.md). For the [Jacobi identity](../../../../../jacobi-identity.md), lift each inner bracket by $[G,H]/h$; the cyclic sum of the outer expressions is the commutator Jacobi identity divided by $h^2$, hence zero. These verifications prove that the graded polynomial ring is a [Poisson algebra](../../../../../poisson-algebra.md). This is the [Poisson bracket from a central deformation parameter](../../../../../poisson-bracket-from-a-central-deformation-parameter.md) construction.

The generators give $\{\xi_i,x_j\}=\delta_{ij}$ and all coordinate-coordinate and symbol-symbol brackets zero. The [Leibniz rule](../../../../../leibniz-rule.md) therefore determines the answer on every polynomial:

$$
\boxed{\{f,g\}=\sum_{i=1}^n
\left(\frac{\partial f}{\partial\xi_i}\frac{\partial g}{\partial x_i}
-\frac{\partial f}{\partial x_i}\frac{\partial g}{\partial\xi_i}\right).}
$$

The sign here follows the chosen convention $[P,Q]=PQ-QP$: in particular $\{\xi_i,x_j\}=\delta_{ij}$, rather than $\{x_i,\xi_j\}=\delta_{ij}$. For homogeneous symbols the bracket has order degree $p+q-1$, and can equivalently be written $\{\sigma_p(P),\sigma_q(Q)\}=\sigma_{p+q-1}([P,Q])$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
