<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For $z=a+b\sqrt d$, let $\bar z=a-b\sqrt d$ denote the [algebraic conjugate](../../../conjugate-element-field-theory.md), not necessarily ordinary complex conjugation when $d>0$. Conjugation respects multiplication, and $z\bar z=a^2-db^2$. Therefore

$$
N(zz')=|(zz')\overline{zz'}|
=|z\bar z|\,|z'\bar z'|
=\boxed{N(z)N(z')}.
$$

If $z$ is a [unit in a ring](../../../unit-in-a-ring.md), choose its inverse $w$ in the same [ring](../../../ring.md). Then $N(z)N(w)=N(1)=1$, and both norms are nonnegative [integers](../../../integer-split.md), forcing $N(z)=1$. Conversely, if $N(z)=1$, then $z\bar z=\pm1$, so $z^{-1}=\pm\bar z$ belongs to the [ring](../../../ring.md). Thus **$z$ is a [unit in a ring](../../../unit-in-a-ring.md) exactly when $N(z)=1$**.

For negative $d$, the equation becomes $a^2+|d|b^2=1$. If $d=-1$, its [integer](../../../integer-split.md) solutions give the four [units](../../../unit-in-a-ring.md) $\pm1,\pm i$. If $d<-1$, the term $|d|b^2$ forces $b=0$, leaving $a=\pm1$. Hence

$$
\boxed{\mathbb Z[\sqrt d]^\times=
\begin{cases}\{1,-1,i,-i\},&d=-1,\\
\{1,-1\},&d<-1.\end{cases}}
$$

For $d=2$, the element $u=1+\sqrt2$ has [field norm](../../../field-norm.md) $|1-2|=1$. Its powers $u^n$, $n\geq0$, are all [units](../../../unit-in-a-ring.md) by [multiplicative function](../../../multiplicative-function.md) and are distinct, since their positive real values strictly increase with $n$. Thus $\mathbb Z[\sqrt2]$ has infinitely many [units](../../../unit-in-a-ring.md). This argument concerns the stated integer-coefficient [ring](../../../ring.md); it does not replace it by a larger [ring](../../../ring.md) of algebraic [integers](../../../integer-split.md).

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2007](../../2007-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
