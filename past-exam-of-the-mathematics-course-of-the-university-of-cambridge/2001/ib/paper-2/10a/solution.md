<h1 id="10a/solution">Solution</h1>

↑ **Parent:** [10A](../10a.md)

A metric space is [totally bounded](../../../../../totally-bounded-space.md) if, for every $\epsilon>0$, finitely many open balls of radius $\epsilon$ cover it. The Bolzano-Weierstrass property here means that every sequence has a subsequence converging to a point of the space, namely [sequential compactness](../../../../../sequentially-compact-space.md).

First suppose that property holds. A [Cauchy sequence](../../../../../cauchy-sequence.md) has a convergent subsequence with limit $x$ in the space. Given $\epsilon>0$, choose an index after which all sequence terms lie within $\epsilon/2$ of each other, and a subsequence term beyond that index within $\epsilon/2$ of $x$. The [triangle inequality](../../../../../triangle-inequality.md) then puts every subsequent term within $\epsilon$ of $x$. Thus the whole Cauchy sequence converges, proving completeness.

If total boundedness failed, some $\epsilon>0$ would admit no finite ball cover. Choose points inductively outside the union of the $\epsilon$-balls about previously chosen points. Distinct sequence terms then have distance at least $\epsilon$. No subsequence can be Cauchy, and therefore none can converge, a contradiction. This proves total boundedness.

Conversely, suppose the space is complete and totally bounded. For any sequence, cover the space by finitely many radius-$2^{-1}$ balls and retain the infinitely many indices in one ball. Within those indices, a finite cover by radius-$2^{-2}$ balls retains an infinite subset in one smaller ball. Repeat with radii $2^{-k}$ to obtain nested infinite index sets $I_k$. Choose increasing indices $n_k\in I_k$. For $l,j\ge k$, both terms lie in the ball selected at step $k$, so

$$
d(x_{n_l},x_{n_j})<2^{1-k}.
$$

The subsequence is Cauchy and completeness makes it converge within the space. Hence **the Bolzano-Weierstrass property is equivalent to completeness plus total boundedness**.

## ↑ Ancestors (10)

1. [10A](../10a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
