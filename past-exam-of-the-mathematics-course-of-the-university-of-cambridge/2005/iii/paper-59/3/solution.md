<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**Perfect identification on every trial is impossible**, because the family contains a nonorthogonal pair. Any physical identification device induces a [POVM](../../../../../positive-operator-valued-measure.md) whose effect $E_i$ corresponds to its declaration of label $i$. Certainty of correct identification would require $\langle\psi_i|E_i|\psi_i\rangle=1$ and $\langle\psi_j|E_i|\psi_j\rangle=0$ for every $j\ne i$.

Since $0\leq E_i\leq I$, the first identity gives $(I-E_i)|\psi_i\rangle=0$, while positivity and the second identity give $E_i|\psi_j\rangle=0$. For example these conclusions follow by writing the zero expectations as squared norms of $(I-E_i)^{1/2}\psi_i$ and $E_i^{1/2}\psi_j$. Thus

$$
\langle\psi_j|\psi_i\rangle=\langle\psi_j|E_i|\psi_i\rangle=0.
$$

Perfect identification would force the entire family to be [orthogonal](../../../../../orthogonal-vectors.md), contrary to the hypothesis. This argument permits ancillas, general measurements and disturbance of the input; it does not assume that the device must preserve the state.

**Unambiguous identification with a nonzero success [probability](../../../../../probability.md) for every input is possible.** Normalize the given kets and let $G_{ij}=\langle\psi_i|\psi_j\rangle$ be their [Gram matrix](../../../../../gram-matrix.md). Their [linear independence](../../../../../linear-independence.md) makes $G$ positive definite. Define reciprocal vectors within their span by

$$
|\chi_i\rangle=\sum_j(G^{-1})_{ji}|\psi_j\rangle.
$$

Then $\langle\psi_k|\chi_i\rangle=\sum_jG_{kj}(G^{-1})_{ji}=\delta_{ki}$, and hence also $\langle\chi_i|\psi_k\rangle=\delta_{ik}$. Put $R=\sum_i|\chi_i\rangle\langle\chi_i|$. It is positive and has finite [operator norm](../../../../../operator-norm.md). Choosing $\epsilon=1/(2\|R\|)>0$, set

$$
\boxed{E_i=\epsilon|\chi_i\rangle\langle\chi_i|,\qquad E_?=I-\epsilon R.}
$$

All these effects are positive, and $E_?\geq I/2$, so they sum to the identity and define a [POVM](../../../../../positive-operator-valued-measure.md). The [Born rule](../../../../../born-rule.md) gives

$$
\boxed{\mathbb P(i\mid\psi_k)=\epsilon\delta_{ik},\qquad
\mathbb P(?\mid\psi_k)=1-\epsilon.}
$$

Thus every label is correct whenever it occurs and every input has the strictly positive success [probability](../../../../../probability.md) $p_k=\epsilon$. This is the [reciprocal-state construction of unambiguous discrimination](../../../../../reciprocal-state-construction-of-unambiguous-discrimination.md).

For an explicit success constant, collect the input kets into a matrix $\Psi$, so $\Psi^\dagger\Psi=G$. Its polar factorization is $\Psi=UG^{1/2}$ with $U^\dagger U=I_N$. The reciprocal columns are $\Psi G^{-1}=UG^{-1/2}$, and therefore $R=UG^{-1}U^\dagger$. Its largest [eigenvalue](../../../../../eigenvalue.md) is $1/\lambda_{\min}(G)$, so one can take $\epsilon=\lambda_{\min}(G)/2$. Since the normalized [Gram matrix](../../../../../gram-matrix.md) has trace $N$, this is at most $1/2$.

To realize the device, use measurement operators $M_i=\sqrt{E_i}$ and $M_?=\sqrt{E_?}$. The map $|v\rangle\mapsto\sum_iM_i|v\rangle|i\rangle+M_?|v\rangle|?\rangle$ preserves [inner products](../../../../../inner-product.md) because the effects sum to $I$. Extend this [linear isometry](../../../../../linear-isometry-of-hilbert-spaces.md) to a unitary on the input and an initially blank ancilla, then projectively measure the ancilla's [orthogonal](../../../../../orthogonal-vectors.md) outcome labels. Its outcome [probabilities](../../../../../probability.md) are precisely those above. This gives a physical [unambiguous quantum state discrimination](../../../../../unambiguous-quantum-state-discrimination.md) device rather than only a formal set of effects.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
