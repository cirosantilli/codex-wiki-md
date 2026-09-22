<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Every element of the $n$-qubit [Pauli group](../../../../../../pauli-group.md) squares to either $1$ or $-1$. If a stabilizer generator $S_j$ had $S_j^2=-1$, closure of the group would put $-1$ in $S$, contrary to the definition. Thus $S_j^2=1$. Since Pauli operators are unitary,

$$
S_j^{-1}=S_j^\dagger,
$$

and $S_j^{-1}=S_j$ proves $S_j=S_j^\dagger$.

If two stabilizers $g,h$ anticommute and a nonzero vector $|\psi\rangle$ belonged to the codespace, then

$$
gh|\psi\rangle=|\psi\rangle,
\qquad
gh|\psi\rangle=-hg|\psi\rangle=-|\psi\rangle,
$$

a contradiction. Hence a nonzero [stabilizer code](../../../../../../stabilizer-code.md) requires $S$ to be Abelian. Its [centralizer of a stabilizer group](../../../../../../centralizer-of-a-stabilizer-group.md) is

$$
\boxed{C(S)=\{P\in\mathcal P_n:Pg=gP\text{ for every }g\in S\}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
