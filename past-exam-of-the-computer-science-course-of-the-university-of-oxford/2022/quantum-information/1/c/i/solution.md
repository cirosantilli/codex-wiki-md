<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

If Alice's [basic measurement](../../../../../../basic-measurement.md) returns a normalized vector $|u\rangle_A$, form Bob's unnormalized conditional vector

$$
|\widetilde\chi_u\rangle_B=(\langle u|_A\otimes I_B)|\chi\rangle_{AB}.
$$

The [Born rule](../../../../../../born-rule.md) and normalization give

$$
\boxed{p_u=\|\widetilde\chi_u\|^2,\qquad
|\chi_u\rangle_B=\frac{|\widetilde\chi_u\rangle_B}{\sqrt{p_u}}\quad(p_u>0).}
$$

The joint [post-measurement state](../../../../../../post-measurement-state.md) is $|u\rangle_A\otimes|\chi_u\rangle_B$. For $|u\rangle_A=\alpha|0\rangle_A+\beta|1\rangle_A$ with real coefficients and $\alpha^2+\beta^2=1$, contraction of the [Bell state](../../../../../../bell-state-split.md) gives

$$
(\langle u|\otimes I)|\phi_+\rangle
=\frac{\alpha|0\rangle+\beta|1\rangle}{\sqrt2},
\qquad p_u=\frac12.
$$

Thus **Bob's normalized conditional state is $\alpha|0\rangle_B+\beta|1\rangle_B$**. For complex coefficients the contraction instead contains their [complex conjugates](../../../../../../complex-conjugate.md); this is the same conjugation underlying [conjugate-basis steering of a Bell pair](../../../../../../conjugate-basis-steering-of-a-bell-pair.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
