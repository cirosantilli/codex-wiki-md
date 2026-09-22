<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Count one copy for each four-element vertex set. It requires six independent edges, so

$$
\boxed{\mu=\mathbb EX=\binom n4\,2^{-6}}.
$$

Distinct copies share an edge exactly when their vertex intersection has size two or three. For each first copy, their numbers are $6\binom{n-4}2$ and $4(n-4)$, respectively. The required union then has eleven or nine edges. Hence the ordered [Janson dependency sum](../../../../../janson-dependency-sum.md) is

$$
\Delta=\binom n4\left(6\binom{n-4}2\,2^{-11}+4(n-4)\,2^{-9}\right).
$$

For large $n$, $\mu=\Theta(n^4)$ and $\Delta=\Theta(n^6)$, so $\Delta\geq\mu$ and $\mu^2/(2\Delta)\geq an^2$ for some constant $a>0$. The second [Janson inequality](../../../../../janson-inequality.md) therefore gives

$$
\boxed{\mathbb P(X=0)\leq e^{-an^2}}.
$$

This is the asserted asymptotic bound. It can also be made valid for every $n\geq4$ by decreasing $a$ to cover the finitely many smaller values, since each then has [probability](../../../../../probability.md) strictly below one of containing no copy. For $n<4$ the event has [probability](../../../../../probability.md) one and no positive exponential bound of this form can hold.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
