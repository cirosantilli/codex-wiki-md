<h1 id="m/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An [absorbing state](../../../../absorbing-state.md) $i$ has $p_{ii}=1$; once reached, the chain never leaves it. For a nonabsorbing initial state, condition on its first transition and use the [Markov property](../../../../markov-property.md):

$$
h_i=\sum_{j\in S}
\mathbb P(X_1=j\mid X_0=i)\,
\mathbb P(\text{eventually hit }1\mid X_1=j)
=\sum_jp_{ij}h_j.
$$

Here $h_1=1$ and $h_4=0$. The other equations are

$$
h_2=\frac13+\frac23h_3,\qquad h_3=\frac14h_2.
$$

Solving gives

$$
\boxed{h_2=\frac25,\qquad h_3=\frac1{10},\qquad h_4=0.}
$$

For absorption into either state one or four, let $e_i$ be the expected number of steps, with $e_1=e_4=0$. [first-step analysis](../../../../first-step-analysis.md) gives

$$
e_2=1+\frac23e_3,\qquad e_3=1+\frac14e_2.
$$

Hence $e_2=2$ and

$$
\boxed{e_3=\frac32.}
$$

The expectation is finite because each transient two-step cycle has [probability](../../../../probability.md) at most $(2/3)(1/4)=1/6$ of remaining transient; the survival tail is geometrically bounded. This also justifies solving the expectation equations without assuming finiteness in advance.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [M](../../m.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
