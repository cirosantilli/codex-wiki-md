<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Stone theorem for one-parameter unitary groups](../../../../../../stone-s-theorem-on-one-parameter-unitary-groups.md) states that every strongly continuous [unitary representation](../../../../../../unitary-representation.md) $U_t$ of $\mathbb R$ is uniquely $U_t=e^{itA}$ for a possibly unbounded [self-adjoint operator](../../../../../../self-adjoint-operator.md) $A$. Its domain is

$$
D(A)=\left\{\xi:\lim_{t\to0}\frac{U_t\xi-\xi}{it}\text{ exists in norm}\right\}.
$$

Conversely every [self-adjoint](../../../../../../self-adjoint-operator.md) $A$ gives such a [group](../../../../../../group-split.md) by the [Borel functional calculus for a normal operator](../../../../../../borel-functional-calculus-for-a-normal-operator.md).

Prove the forward direction by putting $G=iA$, initially defined as the [norm](../../../../../../norm.md) derivative at zero. Its domain is dense: for $f\in C_c^\infty(\mathbb R)$, the [vector](../../../../../../vector.md) $\xi_f=\int f(t)U_t\xi\,dt$ has derivative $G\xi_f=-\int f'(t)U_t\xi\,dt$. Smooth approximate identities make $\xi_f\to\xi$. The [group](../../../../../../group-split.md) law gives $U_tD(G)=D(G)$ and $GU_t=U_tG$ on that domain. Differentiation of preserved [inner products](../../../../../../inner-product.md) shows that $G$ is skew-symmetric, so $A=-iG$ is symmetric.

The derivative operator is closed. Indeed, if $\xi_n\to\xi$ and $G\xi_n\to\eta$, integrate the orbit derivative to obtain

$$
U_t\xi_n-\xi_n=\int_0^tU_sG\xi_n\,ds.
$$

Taking limits gives the same identity with $\xi,\eta$; dividing by $t$ at zero proves $\xi\in D(G)$ and $G\xi=\eta$.

Now define bounded Laplace integrals

$$
R_+\xi=\int_0^\infty e^{-t}U_t\xi\,dt,\qquad
R_-\xi=\int_0^\infty e^{-t}U_{-t}\xi\,dt.
$$

Shifting the integration variable in $U_hR_\pm\xi$ and taking the derivative at zero shows that $R_\pm\xi\in D(G)$ and

$$
GR_+=R_+-I,\qquad GR_-=I-R_-.
$$

Hence $I-G$ and $I+G$ are both surjective. Since $G=iA$, this means $A+iI$ and $A-iI$ are surjective.

Here is why these range conditions establish self-adjointness rather than just symmetry. If $\eta\in D(A^*)$, solve $(A-iI)\xi=(A^*-iI)\eta$. Then $\eta-\xi\in\ker(A^*-iI)=\operatorname{Ran}(A+iI)^\perp=\{0\}$. Thus $D(A^*)\subseteq D(A)$, and symmetry gives equality with $A^*=A$.

The permitted functional calculus now gives $V_t=e^{itA}$. It is unitary, strongly continuous by dominated convergence against spectral measures, and differentiable with derivative $iAV_t\xi$ on $D(A)$. Differentiate $V_{-t}U_t\xi$ for $\xi\in D(A)$; the two derivative terms cancel because both [groups](../../../../../../group-split.md) preserve the domain and commute with their generator. Its value is consequently the constant $\xi$. Density of the domain implies $U_t=V_t$ on all of $H$.

For completeness, the converse and the exact domain follow from the same calculus. If $\xi\in D(A)$, dominated convergence applied to $|(e^{it\lambda}-1)/t|\leq|\lambda|$ gives the derivative $iA\xi$. If that [norm](../../../../../../norm.md) derivative exists, Fatou's lemma applied to its squared [norm](../../../../../../norm.md) gives $\int\lambda^2\,d\langle E_A(\lambda)\xi,\xi\rangle<\infty$, so $\xi\in D(A)$. The derivative characterization also proves uniqueness. Thus

$$
\boxed{\text{strongly continuous unitary groups}\ \longleftrightarrow\ \text{self-adjoint generators}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
