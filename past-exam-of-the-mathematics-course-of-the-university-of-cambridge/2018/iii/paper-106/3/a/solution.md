<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Hahn-Banach separation theorem for two convex sets](../../../../../../hahn-banach-separation-theorem-for-two-convex-sets.md) states that disjoint nonempty [convex sets](../../../../../../convex-set.md) $A,B$ in a real [locally convex space](../../../../../../locally-convex-space.md), with $A$ open, admit a nonzero [continuous linear functional](../../../../../../continuous-linear-functional.md) $\ell$ and $\alpha\in\mathbb R$ such that

$$
\boxed{\ell(a)<\alpha\leq\ell(b)\quad(a\in A,\ b\in B).}
$$

There need not be a positive uniform gap between the two sets.

For a proof, set $C=A-B$. It is open and [convex](../../../../../../convex-function.md), and $0\notin C$. Choose $c_0\in C$, let $V=C-c_0$, and let $p$ be the [Minkowski functional](../../../../../../minkowski-functional.md) of $V$. Because $V$ is open, convex and contains zero, $p$ is a finite [sublinear functional](../../../../../../sublinear-function.md), and $V=\{x:p(x)<1\}$. Put $z=-c_0$. Since $z\notin V$, $p(z)\geq1$. On $\mathbb Rz$ define $\ell_0(tz)=tp(z)$. For $t\geq0$ this equals $p(tz)$; for $t<0$ it is nonpositive and hence at most $p(tz)$. The [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md) extends it to a linear $\ell$ with $\ell\leq p$. Both $p(x)$ and $p(-x)$ are bounded near zero, so this domination makes $\ell$ continuous; it is nonzero because $\ell(z)=p(z)\geq1$. For $c\in C$,

$$
\ell(c)=\ell(c-c_0)-p(z)\leq p(c-c_0)-p(z)<1-p(z)\leq0.
$$

Thus $\ell(a)<\ell(b)$ for every $a\in A,b\in B$. Define $\alpha=\sup_{a\in A}\ell(a)$, which is finite because any fixed $b\in B$ bounds it above. Openness of $A$ and nonzeroness of $\ell$ ensure $\ell(a)<\alpha$ for every $a\in A$, and $\alpha\leq\ell(b)$ for every $b\in B$. This proves the stated separation.

For the sequence criterion, suppose $f\in S_{X^*}$ and $f(x_i)\geq\varrho$. If each $t_i\geq0$, then

$$
\left\|\sum_{i=1}^nt_ix_i\right\|\geq f\left(\sum_{i=1}^nt_ix_i\right)\geq\varrho\sum_{i=1}^nt_i.
$$

Conversely, the assumed inequality implies that every [convex combination](../../../../../../convex-combination.md) of the $x_i$ has norm at least $\varrho$. Hence $D=\{x:\|x\|<\varrho\}$ is disjoint from $C=\operatorname{conv}\{x_i:i\geq1\}$. Apply the separation theorem with the open set $D$ to obtain $\ell\ne0$ and

$$
\ell(c)\geq\sup_{d\in D}\ell(d)=\varrho\|\ell\|\quad(c\in C).
$$

Then $f=\ell/\|\ell\|$ has norm one and satisfies $f(x_i)\geq\varrho$ for every $i$. Therefore

$$
\boxed{\exists f\in S_{X^*},\ \forall i\ f(x_i)\geq\varrho\quad\Longleftrightarrow\quad
\left\|\sum_{i=1}^nt_ix_i\right\|\geq\varrho\sum_{i=1}^nt_i\ \text{for all }n\text{ and }t_i\geq0.}
$$

The PDF confirms the “if and only if” that is garbled in the TeX transcription.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
