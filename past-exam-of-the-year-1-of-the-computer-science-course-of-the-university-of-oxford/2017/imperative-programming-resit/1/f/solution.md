<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use [Binet's formula](../../../../../binet-formula.md) entirely within $\mathbb Q(\sqrt5)$. Set

$$
\phi=(1/2,1/2),\quad\psi=(1/2,-1/2),\quad c=(0,1/5)=1/\sqrt5.
$$

Here pairs mean the rational and radical coefficients. An exact program using the preceding procedures is

```
z = mkRat(0,1); one = mkRat(1,1)
half = mkRat(1,2)
phi = mkIrr(half,half)
psi = mkIrr(half,negRat(half))
c = mkIrr(z,mkRat(1,5))
p = mkIrr(one,z); q = mkIrr(one,z)
for i = 0,...,n-1:
    minusQ = mkIrr(negRat(q.rat),negRat(q.irr))
    OutIrr(mulIrr(c,addIrr(p,minusQ)))
    Out.Ln()
    p = mulIrr(p,phi)
    q = mulIrr(q,psi)
```

At iteration $i$, $p=\phi^i$ and $q=\psi^i$, so the printed value is exactly $F_i$. The irrational coefficient cancels algebraically, and the rational result is an integer. This prints **$F_0,\ldots,F_{n-1}$**; to use the convention $F_1,\ldots,F_n$, initialize `p=phi` and `q=psi`. There are $O(n)$ field operations, with growing arbitrary-precision arithmetic costs kept separate from that count.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [1](../../1.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
