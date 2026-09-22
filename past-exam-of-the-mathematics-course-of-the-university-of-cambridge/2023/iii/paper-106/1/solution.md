<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

[Mazur theorem](../../../../../mazur-theorem.md) says that the weak closure and norm closure of a convex subset of a real or complex normed space coincide. The norm closure is contained in the weak closure because every norm-continuous linear functional is norm-continuous. Conversely, if $x$ is outside the norm closure of a convex set $C$, the [Hahn-Banach separation theorem](../../../../../hahn-banach-separation-theorem.md) gives $f\in X^*$ and a real number $\alpha$ such that

$$
\operatorname{Re}f(x)>\alpha\geq\sup_{y\in C}\operatorname{Re}f(y).
$$

This weakly open separation shows that $x$ is outside the weak closure.

By definition,

$$
x_n\rightharpoonup0
\quad\Longleftrightarrow\quad
f(x_n)\longrightarrow0\quad\text{for every }f\in X^*.
$$

For each $n$, regard $x_n$ as the bounded functional $Jx_n:X^*\to\mathbb F$ given by $Jx_n(f)=f(x_n)$. Pointwise convergence makes the family $(Jx_n)$ pointwise bounded on the Banach space $X^*$. The [Uniform boundedness principle](../../../../../uniform-boundedness-principle.md) gives

$$
\sup_n\|x_n\|=\sup_n\|Jx_n\|<\infty.
$$

Suppose first that $x_n\rightharpoonup0$. Every subsequence indexed by an infinite set $M$ also converges weakly to zero. Thus zero belongs to the weak closure of the convex hull of $\{x_n:n\in M\}$, and Mazur's theorem puts it in its norm closure. This gives the required finite convex combination of norm below any prescribed $\varepsilon$.

Conversely, if weak convergence fails, some $f\in X^*$ and an infinite subsequence satisfy either $\operatorname{Re}f(x_n)\geq\varepsilon$ throughout or $\operatorname{Re}f(x_n)\leq-\varepsilon$ throughout. Every convex combination from that subsequence then has norm at least $\varepsilon/\|f\|$, contradicting the stated property.

Now let the $x_n\in\ell^p$, $1<p<\infty$, have pairwise disjoint supports and satisfy $\|x_n\|_p\leq C$. For $N$ distinct terms,

$$
\left\|\frac1N\sum_{j=1}^N x_{n_j}\right\|_p^p
=\frac1{N^p}\sum_{j=1}^N\|x_{n_j}\|_p^p
\leq C^pN^{1-p}\longrightarrow0.
$$

The convex-combination criterion therefore proves $x_n\rightharpoonup0$. This is [weak convergence of bounded disjointly supported sequences in lp](../../../../../weak-convergence-of-bounded-disjointly-supported-sequences-in-lp.md).

The final implication for a commutative unital [C\*-algebra](../../../../../c-star-algebra.md) is true. By the [Commutative Gelfand--Naimark theorem](../../../../../commutative-gelfand-naimark-theorem.md), $A\cong C(K)$ and its characters are the point evaluations. The hypotheses say that the uniformly bounded functions $a_n$ converge pointwise to zero. Every functional on $C(K)$ is integration against a finite regular measure by the [Riesz-Markov-Kakutani representation theorem](../../../../../riesz-markov-kakutani-representation-theorem.md); the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) gives

$$
\int_Ka_n\,d\mu\longrightarrow0.
$$

**Hence $a_n\rightharpoonup0$.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 106](../../paper-106-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
