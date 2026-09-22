<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The statement $D\!\operatorname{-lim}a_n=a$ means [convergence in density of a sequence](../../../../../convergence-in-density-of-a-sequence.md): for every $\varepsilon>0$, the proportion of $n\leq N$ with $|a_n-a|\geq\varepsilon$ tends to zero. The statement $C\!\operatorname{-lim}a_n=a$ means [Cesaro convergence of a sequence](../../../../../cesaro-convergence-of-a-sequence.md), $N^{-1}\sum_{n=1}^Na_n\to a$.

Suppose $|a_n-a|\leq M$. Splitting into the indices where $|a_n-a|<\varepsilon$ and its complement gives

$$
\frac1N\sum_{n=1}^N|a_n-a|
\leq\varepsilon+M\frac{|\{n\leq N:|a_n-a|\geq\varepsilon\}|}{N}.
$$

Thus density convergence implies Cesaro convergence of the absolute deviations to zero. Conversely, the [Markov inequality](../../../../../markov-inequality.md) gives

$$
\frac{|\{n\leq N:|a_n-a|\geq\varepsilon\}|}{N}
\leq\frac1{\varepsilon N}\sum_{n=1}^N|a_n-a|,
$$

proving the reverse implication.

The [product characterization of weak mixing](../../../../../product-characterization-of-weak-mixing.md) says that if $T$ is weakly mixing, then $T\times S$ is ergodic exactly when $S$ is ergodic; in particular, ergodicity of $T\times T$ characterizes weak mixing.

Suppose $U_Tf=\lambda f$. Unitarity of the [Koopman operator](../../../../../koopman-operator.md) gives $|\lambda|=1$. Weak mixing implies ergodicity, so $|f|$ is almost everywhere constant. On the product,

$$
F(x,y)=f(x)\overline{f(y)}
$$

is invariant under $T\times T$. Since the square is ergodic, $F$ is constant, which forces $f$ to be constant almost everywhere. Thus **there are no nonconstant Koopman eigenfunctions**.

Finally use the density-one correlation characterization of a [weakly mixing measure-preserving transformation](../../../../../weakly-mixing-measure-preserving-transformation.md). For each positive-measure pair $(A,B)$, the integers $n$ for which $\mu(T^{-n}A\cap B)>0$ form a density-one set after discarding finitely many terms; the corresponding sets for $(A,B)$ and $(A,C)$ therefore intersect, proving simultaneous hitting. Conversely, the simultaneous-hitting property is precisely the [simultaneous hitting characterization of weak mixing](../../../../../simultaneous-hitting-characterization-of-weak-mixing.md), so it implies weak mixing.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 108](../../paper-108-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
