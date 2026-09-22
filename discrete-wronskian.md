# Discrete Wronskian

↑ **Parent:** [Linear recurrence relation](linear-recurrence-relation.md)

For two solutions of the [linear recurrence relation](linear-recurrence-relation.md) $x_{n+2}+b_nx_{n+1}+c_nx_n=0$, their discrete [Wronskian](wronskian.md) obeys $W_{n+1}=c_nW_n$. Substitute the recurrence into $p_{n+1}q_{n+2}-p_{n+2}q_{n+1}$: the $b_n$ terms cancel and the remaining expression is $c_n(p_nq_{n+1}-p_{n+1}q_n)$. Iteration gives $W_{n+1}=W_1\prod_{m=1}^nc_m$, including when some $c_m$ vanish. A nonzero discrete Wronskian proves [linear independence](linear-independence.md) of the two solutions.

## ↑ Ancestors (5)

1. [Linear recurrence relation](linear-recurrence-relation.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-2/6b/solution.md)
