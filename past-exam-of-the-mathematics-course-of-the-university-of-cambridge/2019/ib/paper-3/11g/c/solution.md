<h1 id="11g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Factor the equation in the Eisenstein integers:

$$
x^2-x+1=(x+\omega)(x+\omega^2)=y^3.
$$

Let $\pi=1-\omega$. Its norm is $3$, and

$$
\pi^2=-3\omega,
$$

so $3$ is a unit times $\pi^2$. Suppose $x\equiv2\pmod3$, say $x=3k+2$. Since $\omega=1-\pi$,

$$
x+\omega=3(k+1)-\pi.
$$

The first term is divisible by $\pi^2$ and the second has [discrete valuation](../../../../../../discrete-valuation.md) exactly one, so $v_\pi(x+\omega)=1$. Conjugation gives $v_\pi(x+\omega^2)=1$ as well. Consequently

$$
v_\pi(x^2-x+1)=2.
$$

But $v_\pi(y^3)=3v_\pi(y)$ is divisible by three, a contradiction. Hence

$$
\boxed{x\not\equiv2\pmod3}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11G](../../11g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
