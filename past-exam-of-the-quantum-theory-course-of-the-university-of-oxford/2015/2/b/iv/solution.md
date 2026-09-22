<h1 id="2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $\psi$ have energy $E_n$ and put $\gamma=2m\hbar\omega$. The lowering [norm](../../../../../norm.md) formula gives, inductively,

$$
\|(a_-)^j\psi\|^2=\gamma^j\frac{n!}{(n-j)!}\|\psi\|^2,\qquad 0\leq j\leq n.
$$

In particular $(a_-)^n\psi$ is a nonzero [ground state](../../../../../ground-state.md). By the assumed nondegeneracy, it equals $c\psi_0$ for some $c\ne0$.

It remains to show that raising this vector recovers $\psi$, rather than merely another state at the same energy. On an [energy eigenstate](../../../../../energy-eigenstate.md) at $E_n$, factorization gives $a_+a_-\psi=\gamma n\psi$. Iterating the factorization down the ladder yields

$$
(a_+)^n(a_-)^n\psi=\gamma^n n!\,\psi.
$$

Applying $(a_+)^n$ to $(a_-)^n\psi=c\psi_0$ therefore proves

$$
\boxed{\psi=\frac{c}{(2m\hbar\omega)^n n!}(a_+)^n\psi_0.}
$$

For $n=0$ this is the original ground-state assumption. This proves [nondegeneracy propagated by an oscillator ladder](../../../../../nondegeneracy-propagated-by-an-oscillator-ladder.md): every energy [eigenspace](../../../../../eigenspace.md) is one-dimensional if the [ground state](../../../../../ground-state.md) is nondegenerate.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the quantum theory course of the University of Oxford](../../../../split.md)
6. [Quantum theory course of the University of Oxford](../../../../../quantum-theory-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
