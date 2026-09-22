<h1 id="12j/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Consider computations while a terminal block of $b$'s is removed from register $0$. Until that block has disappeared, the available instruction and next state depend on the current state and on the visible $b$, not on the untouched prefix $x$.

Take a block longer than $|Q|$. Record the state after each successive $b$ has been removed. Two records have the same state $q$, by the pigeonhole principle. If the corresponding removed tail lengths are $k\ne\ell$, the same finite instruction [sequences](../../../../../../sequence.md) work in front of every prefix $x$. Thus there are fixed times $t,t'$ such that

$$
\boxed{
C(t,M,xb^k)=(q,x)=C(t',M,xb^\ell)
}
$$

for every word $x$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [12J](../../12j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
