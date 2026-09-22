<h1 id="12j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Two registers suffice. Use register $0$ for the input and register $1$ as a stack of markers.

The finite control first rejects the empty word. While the next input symbol is $a$, remove it from register $0$ and append one marker to register $1$. On seeing the first $b$, enter a second phase. For every $b$ removed from register $0$, remove one marker from register $1$; reject if a marker is unavailable or if an $a$ is encountered in this phase. Accept exactly when both registers become empty simultaneously.

The first phase stores precisely the number of $a$'s, and the second compares it with the number of $b$'s. Register $1$ is the only scratch register, so the construction is a one-register-machine computation in the question's terminology. Therefore

$$
\boxed{\{a^nb^n:n>0\}\text{ is $1$-computable}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
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
