<h1 id="19h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the converse as well as the stated symmetric case, set

$$
a=\mathbb P_i(T_j<T_i),
\qquad
b=\mathbb P_j(T_i<T_j).
$$

Irreducibility and the existence of an invariant probability distribution make the chain positive recurrent, so $a,b>0$. During one return cycle from $i$ to $i$, the chain enters $j$ with probability $a$ and, after entry, makes a geometric number of visits to $j$ with success parameter $b$. Therefore

$$
\mathbb E_iN=\frac ab.
$$

On the other hand, the [stationary cycle occupation formula](../../../../../../stationary-cycle-occupation-formula.md) gives

$$
\mathbb E_iN=\frac{\pi(j)}{\pi(i)}.
$$

Consequently

$$
\frac ab=\frac{\pi(j)}{\pi(i)}.
$$

It follows that

$$
\boxed{a=b\quad\Longleftrightarrow\quad\pi(i)=\pi(j)},
$$

which is precisely the claimed equivalence between symmetry of $i,j$ and equality of their invariant masses.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [19H](../../19h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
