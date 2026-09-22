# Fixed-cardinality binomial coefficient asymptotic

↑ **Parent:** [Binomial coefficient](binomial-coefficient-split.md)

For a fixed nonnegative [integer](integer-split.md) $q$, the number of $q$-element [subsets](subset.md) of an $n$-element [set](set-split.md) satisfies

$$
\binom nq\sim\frac{n^q}{q!}\quad(n\to\infty),
\qquad\binom nq=\Theta(n^q).
$$

For $q\geq1$, divide the product formula for the [binomial coefficient](binomial-coefficient-split.md) by $n^q$:

$$
\frac{\binom nq}{n^q}=\frac1{q!}\prod_{j=0}^{q-1}\left(1-\frac jn\right)\longrightarrow\frac1{q!}.
$$

The empty product gives the same result for $q=0$. For an explicit [big theta notation](big-theta-notation.md) bound, $n\geq2q$ gives $n^q/(2^q q!)\leq\binom nq\leq n^q/q!$. Fixing $q$ is essential: these constants are not uniform when the subset size itself increases with $n$.

## ↑ Ancestors (5)

1. [Binomial coefficient](binomial-coefficient-split.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/discrete-mathematics-continuous-mathematics-and-probability/3/b/solution.md)
