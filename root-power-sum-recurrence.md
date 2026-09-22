# Root power-sum recurrence

↑ **Parent:** [Newton's identities](newton-s-identities.md)

For the [monic polynomial](monic-polynomial.md) $q(z)=z^n-e_1z^{n-1}+\cdots+(-1)^ne_n$, its root power sums satisfy

$$
p_m=e_1p_{m-1}-e_2p_{m-2}+\cdots+(-1)^{n+1}e_np_{m-n},\qquad m>n.
$$

Each root obeys $q(x_i)=0$. Multiplying that equation by $x_i^{m-n}$ and summing over root positions proves the [recurrence relation](recurrence-relation.md). The first $n$ power sums are initialized by [Newton's identities](newton-s-identities.md); their later values require only this fixed-order recurrence. For $q(z)=z^3-6z^2+11z-6$, it gives $p_4=6\cdot36-11\cdot14+6\cdot6=98$. Directly, $1^4+2^4+3^4=98$. No new root-solving step is needed.[§4, p. 3, equations (21)–(33)](rational-univariate-representation-lecture-12-by-jan-verschelde.md)

## ↑ Ancestors (7)

1. [Newton's identities](newton-s-identities.md)
2. [Elementary symmetric polynomial](elementary-symmetric-polynomial.md)
3. [Polynomial](polynomial-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
