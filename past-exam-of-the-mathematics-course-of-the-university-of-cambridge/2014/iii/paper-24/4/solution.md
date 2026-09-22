<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [idele group](../../../../../idele-group.md) is the multiplicative [restricted product](../../../../../restricted-product.md)

$$
J_K=\prod_v'K_v^\times
$$

with respect to $\mathcal O_v^\times$ at the finite [places of a number field](../../../../../place-of-a-number-field.md); $K_v$ is the [completion of a valued field](../../../../../completion-of-a-valued-field.md) at the place $v$. Thus each tuple has nonzero components, and all but finitely many finite components are [units](../../../../../unit-in-a-ring.md). Its [restricted product topology on the idele group](../../../../../restricted-product-topology-on-the-idele-group.md) has basic open sets $\prod_{v\in S}W_v\times\prod_{v\notin S}\mathcal O_v^\times$, where $S$ is finite and contains the infinite places, and each $W_v$ is open in $K_v^\times$. In particular $U_K$ is an open subgroup.

Embed $K^\times$ diagonally. Take a neighbourhood of one whose finite components all lie in $\mathcal O_v^\times$ and whose infinite components satisfy $|x_v-1|<1/2$ in the usual real or complex modulus. A diagonal element there is an algebraic [unit](../../../../../unit-in-a-ring.md) $a$. If $a\ne1$, then $a-1$ is a nonzero [algebraic integer](../../../../../algebraic-integer.md), so its [field norm](../../../../../field-norm.md) is a nonzero integer. But

$$
0<|N_{K/\mathbb Q}(a-1)|=\prod_{\sigma\text{ real}}|\sigma(a)-1|\prod_{\sigma\text{ complex}}|\sigma(a)-1|^2<1,
$$

a contradiction. Thus **$K^\times$ is discrete**. It is also closed: in a topological group, a subgroup with an isolated identity cannot have an external accumulation point, since quotients of two nearby subgroup elements would approach the identity.

Send an [idele](../../../../../idele.md) to its associated [fractional ideal](../../../../../fractional-ideal.md) by

$$
I(x)=\prod_{v\text{ finite}}\mathfrak p_v^{\operatorname{ord}_v(x_v)}.
$$

Only finitely many exponents are nonzero. This homomorphism is onto, by choosing powers of local [uniformizers](../../../../../uniformizer.md), and its kernel is $U_K$. Diagonal elements map to [principal fractional ideals](../../../../../principal-fractional-ideal.md). The resulting quotient gives

$$
\boxed{J_K/(K^\times U_K)\cong\operatorname{Cl}(K).}
$$

It is a topological isomorphism when the [ideal class group](../../../../../ideal-class-group.md) is given the discrete [topology](../../../../../topology-split.md), since $U_K$ is open.

Use normalized local moduli: real modulus, squared complex modulus, and $|\pi_v|_v=(N\mathfrak p_v)^{-1}$ at a finite place. The [idelic modulus](../../../../../idelic-modulus.md) $\|x\|=\prod_v|x_v|_v$ defines $J_K^1=\ker\|\cdot\|$, the [norm-one idele group](../../../../../norm-one-idele-group.md). The [product formula](../../../../../product-formula.md) puts $K^\times$ inside this kernel. Every ideal class has a representative in $J_K^1$, because an infinite component can be rescaled to correct the modulus without altering its [fractional ideal](../../../../../fractional-ideal.md). The compact space $J_K^1/K^\times$ therefore maps continuously onto the discrete [ideal class group](../../../../../ideal-class-group.md). Its image must be finite, proving **$\operatorname{Cl}(K)$ is finite**.

For the [Dirichlet unit theorem](../../../../../dirichlet-s-unit-theorem.md), put $U^1=U_K\cap J_K^1$ and $E=K^\times\cap U^1=\mathcal O_K^\times$. Let $r_1$ count real embeddings and $r_2$ count conjugate complex pairs. Infinite logarithms define a continuous surjection

$$
\ell:U^1\longrightarrow H=\{(t_1,\ldots,t_{r_1+r_2})\in\mathbb R^{r_1+r_2}:\sum_i t_i=0\},
$$

using $\log|x_v|$ at real places and $2\log|x_v|$ at complex places. Its kernel is [compact](../../../../../compact-space.md): it consists of real signs, complex unit circles, and the product of compact finite-place unit groups. More generally the inverse image of a bounded closed subset of $H$ is [compact](../../../../../compact-space.md). Since $E$ is closed and discrete, its intersection with each such inverse image is finite. Hence $\Lambda=\ell(E)$ is discrete in $H$, and the kernel $E\cap\ker\ell$ is a finite group. It is exactly the [roots of unity](../../../../../root-of-unity.md) $\mu(K)$, since every element of a finite multiplicative group has finite order and every [root of unity](../../../../../root-of-unity.md) has all local moduli one.

The image of $U^1$ in $J_K^1/K^\times$ is an open subgroup, hence also closed, and is homeomorphic to $U^1/E$. The assumed compactness therefore makes $U^1/E$ [compact](../../../../../compact-space.md), and its continuous quotient $H/\Lambda$ is [compact](../../../../../compact-space.md). A discrete cocompact subgroup of a real [vector space](../../../../../vector-space-split.md) is a full [Euclidean lattice](../../../../../euclidean-lattice.md), of rank $\dim H=r_1+r_2-1$. Thus $E/\mu(K)\cong\mathbb Z^{r_1+r_2-1}$, and lifting a lattice basis splits off the free factor:

$$
\boxed{\mathcal O_K^\times\cong\mu(K)\times\mathbb Z^{r_1+r_2-1}.}
$$

This derives both finiteness and the unit rank from the stated compactness assumption, rather than assuming either conclusion to prove compactness.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
