<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Interpret the high-success formulation as completeness at least $1-\delta(n)$ and soundness at most $\delta(n)$, where $\delta(n)\leq1/p(n)$ for a growing polynomial $p$. This is the standard error-reduction claim. Literally placing $O$ around a success probability approaching one supplies no useful lower bound; it is the failure probability that must be inverse-polynomially small.

Let $M_x$ be the [quantum verifier acceptance operator](../../../../../../quantum-verifier-acceptance-operator.md) acting on one witness register:

$$
M_x=(I\otimes\langle0|)V_x^\dagger
(I\otimes|1\rangle\langle1|_{\rm out})V_x(I\otimes|0\rangle),
\qquad 0\leq M_x\leq I.
$$

Acceptance on $\rho$ is $\operatorname{Tr}(M_x\rho)$. On a NO instance, $\|M_x\|\leq1/3$; on a YES instance, an honest witness has acceptance at least $2/3$.

Ask for $r$ witness registers, with $r$ odd, run $V_x$ independently on each register with fresh ancillas, and accept a strict majority. The [QMA parallel repetition with entangled witnesses](../../../../../../qma-parallel-repetition-with-entangled-witnesses.md) acceptance operator is

$$
M_x^{(r)}=
\sum_{\substack{z\in\{0,1\}^r\\ |z|>r/2}}
\bigotimes_{j=1}^r M_x^{z_j}(I-M_x)^{1-z_j}.
$$

Diagonalize $M_x$. In the tensor-product eigenbasis, an [eigenvalue](../../../../../../eigenvalue.md) of $M_x^{(r)}$ is the majority probability for independent [Bernoulli random variables](../../../../../../bernoulli-distribution.md) with parameters equal to the selected eigenvalues of $M_x$. On a NO instance every parameter is at most $1/3$. Coupling these variables using independent uniform random numbers shows that their upper majority tail is bounded by the tail with every parameter $1/3$. This bounds the operator norm and therefore covers every supplied witness, including a witness entangled across the registers. No independence assumption about a dishonest witness is being made.

For a valid [Chernoff bound](../../../../../../chernoff-bound.md), if $S$ is a sum of $r$ independent Bernoulli variables of parameter at most $1/3$, [Markov's inequality](../../../../../../markov-inequality.md) applied to $2^S$ yields

$$
\Pr(S\geq r/2)
\leq2^{-r/2}\left(\frac23+\frac13\,2\right)^r
=\left(\frac{2\sqrt2}{3}\right)^r
=e^{-cr},\qquad c=\frac12\ln\frac98>0.
$$

An honest product witness on a YES instance gives independent trials with rejection probability at most $1/3$, so its failure probability has the same bound. The printed concentration bound is not valid as stated: for five trials at parameter $1/3$, the upper-majority probability is $17/81>e^{-5/3}$. The valid bound above suffices for a rigorous proof.

Choose the next odd integer above $c^{-1}\ln p(n)$. Then

$$
\boxed{\text{completeness}\geq1-\frac1{p(n)},\qquad
\text{soundness}\leq\frac1{p(n)}.}
$$

The witness length and circuit size increase by only $O(\log p(n))$; the majority calculation has polynomial overhead. Conversely, inverse-polynomial failure probability is at most $1/3$ for all sufficiently large input lengths. Finitely many smaller lengths can be handled by hard-wired verifiers, giving the usual constants. Hence **the two definitions give the same class QMA**. The same [QMA error reduction](../../../../../../qma-error-reduction.md) argument also yields exponentially small failure with polynomially many copies.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
