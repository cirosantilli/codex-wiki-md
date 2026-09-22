<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $c=\bigcup G$ and $d(n)=c(2n)$. Define

$$
H=\{p\in\operatorname{Fn}(\omega,2)^M:p\subseteq d\}.
$$

This is a filter: restrictions of finite pieces of $d$ remain in $H$, and the union of two members is a common stronger condition.

To prove genericity, take a dense set $D\in M$. Let $E_D$ consist of conditions $q\in\operatorname{Fn}(\omega,2)$ for which some $p\in D$ satisfies

$$
p(n)=q(2n)\qquad(n\in\operatorname{dom}p).
$$

The set $E_D$ is dense. Indeed, given $q$, first read its finitely many assigned even coordinates as a condition $p_0$ on $\omega$. Choose $p\le p_0$ in $D$, and extend $q$ by setting $q(2n)=p(n)$ at the remaining coordinates of $p$. Since $E_D\in M$, the [generic filter](../../../../../../generic-filter.md) $G$ meets it. For $q\in G\cap E_D$, the corresponding $p\in D$ is a finite subfunction of $d$, so $p\in H\cap D$.

Thus $H$ meets every dense subset belonging to $M$. Moreover, each singleton $\{(n,d(n))\}$ belongs to $H$, and hence

$$
\boxed{H\text{ is }\operatorname{Fn}(\omega,2)\text{-generic over }M,qquad\bigcup H=d.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 128](../../../paper-128-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
