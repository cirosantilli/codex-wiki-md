# Recursive construction of a compositional inverse

↑ **Parent:** [Compositional inverse of a formal power series](compositional-inverse-of-a-formal-power-series.md)

Let $R$ be a commutative unital [ring](ring.md) and $f(T)=a_1T+a_2T^2+\cdots$ with $a_1$ a [unit](unit-in-a-ring.md). Set $g(T)=\sum_{n\ge1}b_nT^n$. The coefficient of $T$ in $f(g(T))$ gives $b_1=a_1^{-1}$. At every degree $n>1$, the coefficient is $a_1b_n$ plus an expression involving only $b_1,\ldots,b_{n-1}$; choose $b_n$ to cancel that expression. This gives a unique right [compositional inverse of a formal power series](compositional-inverse-of-a-formal-power-series.md).

Similarly, the coefficient of $T^n$ in $h(f(T))$ is $a_1^n h_n$ plus previously fixed terms, so the same recursion gives a left inverse $h$. Composition of zero-constant-term [formal power series](formal-power-series.md) is associative, since every coefficient involves finitely many terms. Therefore $h=h\circ(f\circ g)=(h\circ f)\circ g=g$, proving $f\circ g=g\circ f=T$.

## ↑ Ancestors (9)

1. [Compositional inverse of a formal power series](compositional-inverse-of-a-formal-power-series.md)
2. [Formal power series](formal-power-series.md)
3. [Commutative ring](commutative-ring.md)
4. [Ring](ring.md)
5. [Commutative algebra](commutative-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-27/2/i/solution.md)
