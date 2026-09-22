<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

We prove the required [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) for a [seminorm](../../../../../seminorm.md) directly. First suppose the [vector space](../../../../../vector-space-split.md) is real. At an intermediate extension stage, let $g:E\to\mathbb R$ be a [linear functional](../../../../../linear-functional.md) with $|g(y)|\leq p(y)$, and let $z\notin E$. Extending to $E+\mathbb Rz$ amounts to choosing $c=f(z)$. The upper domination $f\leq p$ requires

$$
\sup_{y\in E}\{g(y)-p(y-z)\}\ \leq c\leq\ \inf_{w\in E}\{p(w+z)-g(w)\}.
$$

The interval is nonempty: for all $y,w\in E$,

$$
g(y)+g(w)=g(y+w)\leq p(y+w)\leq p(y-z)+p(w+z).
$$

Its endpoints are finite since inserting zero gives bounds $-p(z)$ and $p(z)$, while every lower candidate is below every upper candidate. Choose $c$ in the interval and put $f(y+tz)=g(y)+tc$. For $t>0$, the upper bound with $w=y/t$ proves $f(y+tz)\leq p(y+tz)$. For $t<0$, writing $s=-t>0$ and applying the lower bound with $y/s$ proves the same inequality. The case $t=0$ is already known. Applying this domination to $-x$ and using $p(-x)=p(x)$ gives $|f(x)|\leq p(x)$.

Partially order all dominated [linear functional](../../../../../linear-functional.md) extensions of the original $g$ by extension of their domains and values. They form a nonempty set. The union along any chain is a well-defined dominated [linear functional](../../../../../linear-functional.md) on a [vector subspace](../../../../../vector-subspace.md), so every chain has an upper bound. The [Zorn lemma](../../../../../zorn-s-lemma.md) gives a maximal extension. If its domain were not $X$, the preceding one-dimensional construction would enlarge it, a contradiction. Thus the required extension exists on $X$.

For a complex [vector space](../../../../../vector-space-split.md), apply the proved real result to $\operatorname{Re}g$ on the underlying real [vector subspace](../../../../../vector-subspace.md). Let $U:X\to\mathbb R$ be the resulting real [linear functional](../../../../../linear-functional.md), with $|U(x)|\leq p(x)$, and set

$$
f(x)=U(x)-iU(ix).
$$

It is additive and real-linear, and $f(ix)=if(x)$, so it is complex-linear. On $Y$, the identity $\operatorname{Re}g(iy)=-\operatorname{Im}g(y)$ proves $f(y)=g(y)$. Choose $\alpha$ with $|\alpha|=1$ and $\alpha f(x)=|f(x)|$ when $f(x)\ne0$. Then

$$
|f(x)|=\operatorname{Re}f(\alpha x)=U(\alpha x)\leq p(\alpha x)=p(x).
$$

The bound is immediate if $f(x)=0$. This proves the real and complex [seminorm](../../../../../seminorm.md) forms of [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) without invoking any version of that theorem.

For the [distance to a set](../../../../../distance-to-a-set.md) assertion, let $d=d(z,Y)>0$. Define on $Y+\mathbb Kz$ the [linear functional](../../../../../linear-functional.md) $g(y+\alpha z)=\alpha d$. The decomposition is unique because $z\notin Y$, and for $\alpha\ne0$,

$$
|g(y+\alpha z)|=|\alpha|d
\leq|\alpha|\|z+y/\alpha\|=\|y+\alpha z\|.
$$

For $\alpha=0$ the bound is immediate. Apply the just-proved [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) with $p(x)=\|x\|$ to get $f\in X^*$, $f|_Y=0$, $f(z)=d$, and $\|f\|\leq1$. Choose $y_n\in Y$ with $\|z-y_n\|\to d$. Since

$$
d=|f(z-y_n)|\leq\|f\|\|z-y_n\|,
$$

and $d>0$, passage to the limit gives $\|f\|\geq1$. Thus **$\boxed{f|_Y=0,\quad f(z)=d(z,Y),\quad\|f\|=1}$**. This version of the [Hahn-Banach distance formula](../../../../../hahn-banach-distance-formula.md) needs neither a closed $Y$ nor an attained [distance to a set](../../../../../distance-to-a-set.md).

For the [Banach limit](../../../../../banach-limit.md) construction below, take the real [l-infinity sequence space](../../../../../l-infinity-sequence-space.md), let $S(x_1,x_2,\ldots)=(x_2,x_3,\ldots)$ be its [left shift on bounded sequences](../../../../../left-shift-on-bounded-sequences.md), put $Y=(I-S)\ell^\infty$, and let $\mathbf1=(1,1,\ldots)$. This is a [vector subspace](../../../../../vector-subspace.md) and its [distance to a set](../../../../../distance-to-a-set.md) from $\mathbf1$ determines the construction.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
