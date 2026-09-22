# Weighted argument principle

↑ **Parent:** [Argument principle](argument-principle.md)

The boundary can recover more than a count. Under the hypotheses of the [argument principle](argument-principle.md), let $h$ be a [holomorphic function](holomorphic-function.md) on a [neighborhood](neighbourhood-mathematics.md) of the contour and its interior. If the enclosed [zeros of a function](zero-of-a-function.md) are $a_j$ with [zero multiplicities](multiplicity-of-a-zero.md) $m_j$ and the enclosed [poles](pole.md) are $b_k$ of orders $n_k$, then

$$
\frac1{2\pi i}\oint_\gamma h(z)\frac{f'(z)}{f(z)}\,dz=\sum_jm_jh(a_j)-\sum_kn_kh(b_k).
$$

Multiplying the local [logarithmic derivative](logarithmic-derivative.md) by $h$ changes its [residue](residue.md) from $m_j$ to $m_jh(a_j)$, or from $-n_k$ to $-n_kh(b_k)$. The [residue theorem](residue-theorem.md) then gives the identity. Choosing $h=1$ recovers the [argument principle](argument-principle.md); choosing $h(z)=z$ gives the sum of the enclosed zero locations minus the sum of the enclosed pole locations, both counted with [zero multiplicities](multiplicity-of-a-zero.md) or pole orders.[§1.10(iv), equation 1.10.10](nist-digital-library-of-mathematical-functions/1-algebraic-and-analytic-methods.md)

For the [rational function](rational-function.md) in [argument principle for a rational function](argument-principle-for-a-rational-function.md), the $h(z)=z$ integral is $2(1/4)-(-1/2)=1$. Adding the known pole location $-1/2$ back gives a zero-location sum of $1/2$. Dividing by the zero count two gives **the arithmetic mean of the enclosed zeros, with multiplicity, as $1/4$**. Choosing $h(z)=z^k$ similarly gives the difference between the [power-sum symmetric polynomials](power-sum-symmetric-polynomial.md) evaluated on the enclosed zero and pole locations, repeating each location according to its multiplicity or order. These identities let boundary information constrain both the number and aggregate locations of enclosed [zeros of a function](zero-of-a-function.md).

## ↑ Ancestors (6)

1. [Argument principle](argument-principle.md)
2. [Complex analysis](complex-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [1 Algebraic and Analytic Methods](nist-digital-library-of-mathematical-functions/1-algebraic-and-analytic-methods.md)
