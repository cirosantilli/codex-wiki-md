<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the metric in the question and fix the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) convention $\epsilon_{0123}=+1$. A consistent choice of rotation [Lie algebra generators](../../../../../lie-algebra-generator.md) is

$$
\boxed{J_1=M^{23},\qquad J_2=M^{31},\qquad J_3=M^{12}.}
$$

Substituting the indices into the printed [Poincare algebra](../../../../../poincare-algebra.md) gives

$$
[J_1,J_2]=[M^{23},M^{31}]=\eta^{33}M^{21}
=-M^{21}=M^{12}=J_3.
$$

The other cyclic brackets follow the same way. The negative spatial metric and antisymmetry of $M^{\rho\sigma}$ both enter this sign.

The printed brackets are real [Lie algebra](../../../../../lie-algebra-split.md) brackets, without the factor $i$ used for ordinary [commutators](../../../../../commutator.md) of Hermitian quantum observables. We use those brackets for the algebraic verifications. For physical eigenvalues below, angular momentum is Hermitian, its [spin](../../../../../spin.md) projection is the real number $j_3$, and $\hbar=1$. In that quantum convention the ordinary operator [commutators](../../../../../commutator.md) are $i$ times the displayed brackets. This distinction prevents identifying a real [spin](../../../../../spin.md) projection with an anti-Hermitian [matrix](../../../../../matrix.md) eigenvalue.

In the [universal enveloping algebra](../../../../../universal-enveloping-algebra.md), translations commute. The [Pauli-Lubanski pseudovector](../../../../../pauli-lubanski-pseudovector.md) therefore satisfies

$$
W_\mu P^\mu=\frac12\epsilon_{\mu\nu\rho\tau}M^{\nu\rho}P^\tau P^\mu=0.
$$

For fixed $\nu,\rho$, the product of momenta is symmetric in $\mu,\tau$ while the epsilon coefficient is antisymmetric in them. There is no need to commute the Lorentz generator through the momenta.

Using the [commutator derivation identity](../../../../../commutator-derivation-identity.md) and the mixed bracket,

$$
\begin{aligned}
[W_\mu,P^\sigma]
&=\frac12\epsilon_{\mu\nu\rho\tau}
\bigl(\eta^{\rho\sigma}P^\nu-\eta^{\nu\sigma}P^\rho\bigr)P^\tau\\
&=\epsilon_{\mu\nu\rho\tau}\eta^{\rho\sigma}P^\nu P^\tau=0.
\end{aligned}
$$

The two terms become equal after swapping $\nu,\rho$, and the last expression vanishes by antisymmetry in $\nu,\tau$. In the Hermitian observable convention, the calculation has one overall extra $i$ and still vanishes. Thus **$W_\mu$ preserves each momentum eigenspace**.

For the specified epsilon orientation, two useful component identities are

$$
W_0=J_1P^1+J_2P^2+J_3P^3,
\qquad W_3=-J_3P^0+M^{02}P^1-M^{01}P^2.
$$

The order displayed matters: the momentum operator is on the right, so it can act first on the momentum eigenstate. At rest, $p^\mu=(m,0,0,0)$, and on a [spin](../../../../../spin.md) state with $J_3|j,j_3\rangle=j_3|j,j_3\rangle$ these give

$$
\boxed{W_0|\psi\rangle=0,\qquad W_3|\psi\rangle=-mj_3|\psi\rangle.}
$$

These are [massive rest-frame Pauli-Lubanski eigenvalues](../../../../../massive-rest-frame-pauli-lubanski-eigenvalues.md). The raised component would be $W^3=+mj_3$; confusing $W_3$ with $W^3$ reverses the answer.

[Helicity](../../../../../helicity.md) is the projection of [spin angular momentum](../../../../../spin.md), or equivalently the rotation generator acting internally, along the momentum direction:

$$
h=\frac{\mathbf J\cdot\mathbf p}{|\mathbf p|}.
$$

For the momentum $p^\mu=(k,0,0,k)$ with $k>0$, the [helicity](../../../../../helicity.md) operator is $J_3$. Hence a [helicity](../../../../../helicity.md)-$j_3$ state has

$$
\boxed{W_0|\psi\rangle=kj_3|\psi\rangle,\qquad
W_3|\psi\rangle=-kj_3|\psi\rangle.}
$$

The result uses only the two longitudinal components and does not need a separate assumption about the transverse little-group generators. These [massless longitudinal Pauli-Lubanski eigenvalues](../../../../../massless-longitudinal-pauli-lubanski-eigenvalues.md) agree with $W^\mu=j_3P^\mu$ for ordinary finite-[helicity](../../../../../helicity.md) representations.

Finally, at rest the contraction is $mW_0=0$. For the chosen null momentum it is $k(W_0+W_3)$, whose two eigenvalues cancel. Thus **both results obey $W_\mu P^\mu=0$**. Reversing the epsilon orientation reverses all $W$ eigenvalues together; it leaves both identities and both consistency checks intact. For a literal anti-Hermitian derived representation $\rho$ of the printed real algebra, write $H_X=i\rho(X)$ for the Hermitian observable. Since $W_\mu$ is bilinear in generators, its abstract enveloping-algebra image is $\rho(W_\mu)=-W_{\mu,\mathrm{phys}}$. Thus the corresponding formal-image eigenvalues, if that convention is intended, are

$$
\boxed{\text{rest}:\ (\rho(W_0),\rho(W_3))=(0,+mj_3),\qquad
\text{null}:\ (\rho(W_0),\rho(W_3))=(-kj_3,+kj_3).}
$$

Here $\rho(P^\mu)$ has eigenvalue $-ip^\mu$, while $p^\mu$ and $j_3$ themselves remain real physical labels. This is the same result after the [Hermitian quantum generator convention](../../../../../hermitian-quantum-generator-convention.md) is applied to both factors, not an inconsistent choice of [spin](../../../../../spin.md) sign. Both the Hermitian-observable and literal anti-Hermitian interpretations are consequently specified.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
