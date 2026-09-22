<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [primitive recursive functions](../../../../../../primitive-recursive-function.md) are the smallest collection containing zero functions, successor $S(n)=n+1$, and coordinate projections, and closed under composition and [primitive recursion](../../../../../../primitive-recursion.md). The recursion scheme forms $F$ from already constructed functions $G,H$ by

$$
F(\mathbf x,0)=G(\mathbf x),\qquad
F(\mathbf x,n+1)=H(\mathbf x,n,F(\mathbf x,n)).
$$

Constants follow by composing successor with zero. Define addition, multiplication and exponentiation successively by

$$
A(m,0)=m,\quad A(m,n+1)=S(A(m,n)),
$$



$$
M(m,0)=0,\quad M(m,n+1)=A(M(m,n),m),
$$



$$
E(m,0)=1,\quad E(m,n+1)=M(E(m,n),m).
$$

At each stage the initial and step functions are compositions of [primitive recursive functions](../../../../../../primitive-recursive-function.md) already available. Induction on $n$ gives $A(m,n)=m+n$, $M(m,n)=mn$, and $E(m,n)=m^n$, with the recursive convention $0^0=1$. Composition with the second projection now gives

$$
\boxed{f(m,n)=A(E(m,n),n)=m^n+n\text{ is primitive recursive}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
