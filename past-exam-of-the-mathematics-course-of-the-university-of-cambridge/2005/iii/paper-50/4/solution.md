<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use a finite-dimensional complex [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md), or the complexification of its compact real form, as required for the root construction. Choose a [Cartan subalgebra](../../../../../cartan-subalgebra.md) with basis $H_1,\ldots,H_r$. Simultaneous diagonalization of its adjoint action gives the [root-space decomposition](../../../../../root-space-decomposition.md)

$$
L=\mathfrak h\oplus\bigoplus_{\alpha\in\Phi}L_\alpha,\qquad[H_i,E_\alpha]=\alpha(H_i)E_\alpha.
$$

The nonzero weights are the [roots of a root system](../../../../../root-of-a-root-system.md); each [root space](../../../../../root-space.md) is one-dimensional in this setting, and roots occur in opposite pairs. This supplies the Cartan and root-vector basis.

The [Jacobi identity](../../../../../jacobi-identity.md) gives

$$
[H_i,[E_\alpha,E_\beta]]=(\alpha(H_i)+\beta(H_i))[E_\alpha,E_\beta].
$$

If the bracket is nonzero and $\alpha+\beta\ne0$, it is a nonzero vector in the [root space](../../../../../root-space.md) of weight $\alpha+\beta$, so that sum is a root. **The printed implication needs the opposite-root exception:** for $\beta=-\alpha$, $[E_\alpha,E_{-\alpha}]$ can be a nonzero Cartan element, while zero is not a root. The supplied simple-root commutator itself gives this counterexample. This is the [root bracket and the opposite-root exception](../../../../../root-bracket-and-the-opposite-root-exception.md).

Choose a real linear functional nonzero on every root; [positive roots](../../../../../positive-root.md) are those on which it is positive, and [negative roots](../../../../../negative-root.md) are their negatives. The [simple roots](../../../../../simple-root.md) are [positive roots](../../../../../positive-root.md) not decomposable into two [positive roots](../../../../../positive-root.md). They form a basis $\alpha_1,\ldots,\alpha_r$ of the root span, and every root is an integer combination

$$
\alpha=\sum_i m_i\alpha_i,
$$

with all $m_i\ge0$ for a [positive root](../../../../../positive-root.md) and all $m_i\le0$ for a [negative root](../../../../../negative-root.md). [Positive roots](../../../../../positive-root.md) can be decomposed repeatedly until [simple roots](../../../../../simple-root.md) remain; the finite root set makes this procedure terminate.

For $i\ne j$, $\alpha_j-\alpha_i$ has simple-root coefficients of both signs and is not a root. It is also nonzero, so the root-space bracket rule gives

$$
\boxed{[E_i^-,E_j^+]=0.}
$$

The operators $E_i^\pm,\widehat H_i$ have the [SU(2) Lie algebra](../../../../../su-2-lie-algebra.md) normalization $\widehat H_i=2J_3$, $E_i^\pm=J_\pm$. In a finite-dimensional representation, a vector killed by $E_i^-$ is a lowest-weight vector in its SU(2) summands. If its $\widehat H_i$ value is $-\lambda$, those summands have spin $\lambda/2$, so

$$
\boxed{\lambda\in\mathbb Z_{\ge0},\qquad(E_i^+)^{\lambda+1}|\psi\rangle=0.}
$$

One can also read the termination from successive raising coefficients $\sqrt{(\lambda-k)(k+1)}$ starting at the lowest weight.

Apply this result in the finite-dimensional [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md), taking the lowest-weight vector to be $E_j^+$. The vanishing bracket just proved is its lowering condition. If $[\widehat H_i,E_j^+]=a_{ij}E_j^+$, the lowest-weight result forces $a_{ij}=-n_{ij}$ with $n_{ij}$ a nonnegative integer. It also yields

$$
\boxed{[\widehat H_i,E_j^+]=-n_{ij}E_j^+,\qquad(\operatorname{ad}E_i^+)^{n_{ij}+1}E_j^+=0\quad(i\ne j).}
$$

The last identity is exactly the requested nested commutator. This is the [SU(2) proof of the Serre relations](../../../../../su-2-proof-of-the-serre-relations.md), and the identities are the [Serre relations](../../../../../serre-relations.md) in these [Chevalley basis](../../../../../chevalley-basis.md) conventions.

To construct a [highest-weight representation](../../../../../highest-weight-representation.md), start from its [highest-weight vector](../../../../../highest-weight-vector.md) and apply negative-root operators. Fix an order on the [negative roots](../../../../../negative-root.md). The [Poincaré-Birkhoff-Witt theorem](../../../../../poincare-birkhoff-witt-theorem.md) gives spanning vectors

$$
E_{-\beta_1}^{k_1}\cdots E_{-\beta_N}^{k_N}|w\rangle,\qquad k_i\ge0,
$$

of weight $w-\sum_i k_i\beta_i$. The spanning assertion follows by commuting all negative-root operators to the left, Cartan operators to the middle and positive-root operators to the right; commutators supply lower-order words, positive operators kill the [highest-weight vector](../../../../../highest-weight-vector.md) and Cartan operators act there by scalars. In the finite-dimensional [highest-weight representation](../../../../../highest-weight-representation.md), impose the simple-root string relations $(E_i^-)^{w_i+1}|w\rangle=0$ and the commutator/[Serre relations](../../../../../serre-relations.md). At each weight retain a linearly independent set of the resulting words, discarding zero words and dependencies. This gives a basis, with separate independent vectors retained when a weight has multiplicity greater than one. The construction is finite in the assumed finite-dimensional representation; treating all lowering words as automatically independent would overcount.

For [SU(3)](../../../../../su-3-group.md), put $e_i=E_i^+$, $f_i=E_i^-$ and $h_i=\widehat H_i$. The off-diagonal Cartan entries are minus one, so the [Serre relations](../../../../../serre-relations.md) give $(\operatorname{ad}e_1)^2e_2=(\operatorname{ad}e_2)^2e_1=0$. With $e_3=[e_1,e_2]$, these imply

$$
[e_3,e_1]=[e_3,e_2]=0.
$$

For $f_3=-[f_1,f_2]$, expand the commutator using [Jacobi identity](../../../../../jacobi-identity.md) and the distinct-root brackets:

$$
[f_3,e_1]=-[f_1,[f_2,e_1]]+[f_2,[f_1,e_1]]=[f_2,-h_1]=f_2,
$$

since $[h_1,f_2]=f_2$. Similarly,

$$
[h_1,e_3]=[[h_1,e_1],e_2]+[e_1,[h_1,e_2]]=2e_3-e_3=e_3,
$$

and the same calculation on $f_3$ gives $[h_1,f_3]=-f_3$. Thus

$$
\boxed{[E_3^-,E_1^+]=E_2^-,\qquad[\widehat H_1,E_3^\pm]=\pm E_3^\pm.}
$$

These signs also agree with the explicit model $e_1=E_{12}$, $e_2=E_{23}$, $e_3=E_{13}$, $f_1=E_{21}$, $f_2=E_{32}$, $f_3=E_{31}$.

For the [SU(3) Casimir in Chevalley generators](../../../../../su-3-casimir-in-chevalley-generators.md), set

$$
P=h_1^2+h_2^2+h_1h_2+3(h_1+h_2),\qquad C=P+3(f_1e_1+f_2e_2+f_3e_3).
$$

Using $[h_1,e_1]=2e_1$, $[h_2,e_1]=-e_1$, and putting Cartan elements on the left, the four terms of $[P,e_1]$ are

$$
[h_1^2,e_1]=(4h_1-4)e_1,\quad[h_2^2,e_1]=(-2h_2-1)e_1,\quad[h_1h_2,e_1]=(-h_1+2h_2+2)e_1,\quad[3(h_1+h_2),e_1]=3e_1.
$$

Their sum is $3h_1e_1$. The remaining terms give

$$
[f_1e_1,e_1]=-h_1e_1,\qquad[f_2e_2,e_1]=-f_2e_3,\qquad[f_3e_3,e_1]=f_2e_3.
$$

The last two cancel, so $[C,e_1]=3h_1e_1-3h_1e_1=0$. Also $h_1$ commutes with every Cartan polynomial and with each $f_ne_n$: their raising and lowering weights cancel in the product. Hence

$$
\boxed{[C,E_1^+]=[C,\widehat H_1]=0.}
$$

On $|w_1,w_2\rangle$, $e_1$ and $e_2$ vanish and therefore $e_3=[e_1,e_2]$ vanishes as well. All three $f_ne_n$ terms consequently give zero, leaving

$$
\boxed{C|w_1,w_2\rangle=\bigl[w_1^2+w_2^2+w_1w_2+3(w_1+w_2)\bigr]|w_1,w_2\rangle.}
$$

The paper's normalization is $C=3C_2$ relative to the conventional [SU(3) quadratic Casimir eigenvalue](../../../../../su-3-quadratic-casimir-eigenvalue.md). For example it gives $4$ in the fundamental representation, $9$ in the octet and $18$ in the decuplet.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
