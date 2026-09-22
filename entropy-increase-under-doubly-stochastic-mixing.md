# Entropy increase under doubly stochastic mixing

↑ **Parent:** [Doubly stochastic matrix](doubly-stochastic-matrix.md)

Let $A$ be a [doubly stochastic matrix](doubly-stochastic-matrix.md), let $q$ be a [probability vector](probability-vector.md), and put $w=Aq$. In row $i$ with $w_i>0$, define $r_i(j)=a_{ij}q_j/w_i$ on the [support](support.md) where $a_{ij}>0$. The positive row entries $\alpha_i=(a_{ij})$ form a [probability vector](probability-vector.md). Expanding [relative entropy](kullback-leibler-divergence.md) and using the column sums gives

$$
H(w)-H(q)=\sum_{i:w_i>0}w_i d(r_i,\alpha_i)\geq0.
$$

Zero-output rows contribute zero because all their $a_{ij}q_j$ vanish. The row sums supply the normalized comparison laws, while the column sums preserve the input [entropy](information-entropy-split.md) contribution. [Equality](equality-mathematics.md) holds exactly when $q_j=w_i$ for every positive [matrix](matrix.md) entry $a_{ij}$, including the automatic zero values in zero-output rows.

## ↑ Ancestors (9)

1. [Doubly stochastic matrix](doubly-stochastic-matrix.md)
2. [Matrix](matrix.md)
3. [Linear map](linear-map.md)
4. [Vector space](vector-space-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-communication-theory-course-of-the-university-of-oxford/2011/1/c/solution.md)
