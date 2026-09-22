<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

Fix $\alpha\in\Omega$. If $\beta=g\alpha$, then normality of $H$ gives

$$
g(H\alpha)=(gHg^{-1})(g\alpha)=H\beta.
$$

Thus the transitive [group action](../../../../../group-action.md) of $G$ permutes the [orbits of a group action](../../../../../orbit-of-a-group-action.md) of $H$, so all $H$-orbits have the same cardinality $d$. They partition the prime-sized set $\Omega$, hence $d$ divides $|\Omega|$. The only possibilities are $d=1$ and $d=|\Omega|$. The first would make every element of $H$ fix every point, contrary to the assumption that $H$ acts nontrivially. Therefore $d=|\Omega|$ and

$$
\boxed{H\text{ acts transitively on }\Omega}.
$$

Now suppose $H\cap G_\alpha=\{1\}$. Define the [orbit map](../../../../../orbit-map.md)

$$
\theta:H\longrightarrow\Omega,
\qquad
\theta(h)=h\alpha.
$$

It is surjective by transitivity of $H$. If $\theta(h_1)=\theta(h_2)$, then $h_2^{-1}h_1\in H\cap G_\alpha$, so $h_1=h_2$; hence $\theta$ is bijective. For $k\in G_\alpha$,

$$
\theta(khk^{-1})
=khk^{-1}\alpha
=kh\alpha
=k\theta(h).
$$

**Thus $\theta$ is an [equivariant map](../../../../../equivariant-map.md): [conjugation](../../../../../conjugation.md) by $G_\alpha$ on $H$ corresponds exactly to the given action of $G_\alpha$ on $\Omega$.**

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
