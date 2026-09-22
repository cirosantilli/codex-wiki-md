<h1 id="11d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Rolle theorem](../../../../../../rolle-theorem.md): if $f$ is continuous on $[a,b]$, differentiable on $(a,b)$, and $f(a)=f(b)$, then $f'(c)=0$ for some $c\in(a,b)$. Indeed, the [extreme value theorem](../../../../../../extreme-value-theorem.md) gives a maximum and minimum. If both occur only at the endpoints then $f$ is constant; otherwise an interior extremum $c$ satisfies $f'(c)=0$ by comparing the two-sided difference quotients.

[Mean value theorem](../../../../../../mean-value-theorem.md): if $f$ is continuous on $[a,b]$ and differentiable on $(a,b)$, then some $c\in(a,b)$ satisfies

$$
f'(c)=\frac{f(b)-f(a)}{b-a}.
$$

Apply Rolle's theorem to

$$
h(x)=f(x)-f(a)-\frac{f(b)-f(a)}{b-a}(x-a),
$$

which has $h(a)=h(b)=0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11D](../../11d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
