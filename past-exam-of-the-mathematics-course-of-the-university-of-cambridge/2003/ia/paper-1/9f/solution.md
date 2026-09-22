<h1 id="9f/solution">Solution</h1>

↑ **Parent:** [9F](../9f.md)

To prove the [Archimedean property](../../../../../archimedean-property.md), suppose the positive integers were bounded above in $\mathbb R$. By the [least upper bound axiom](../../../../../least-upper-bound-property.md) they would have a finite [supremum](../../../../../supremum.md) $s$. Since $s-1$ is not an upper bound, some positive integer $k$ satisfies $k>s-1$. Then the positive integer $k+1>s$, contradicting the definition of $s$. Thus the positive integers are unbounded. Equivalently, for any positive real $a,b$, some positive integer $n$ satisfies $na>b$, by applying unboundedness to $b/a$.

For fixed $m$, put $r_m=\cos^2(m!\pi x)$. The standard properties needed are $0\le\cos^2 t\le1$, and $\cos^2 t=1$ exactly when $t\in\pi\mathbb Z$. If $0\le r<1$, then $r^n\to0$; for $0<r<1$ this also follows from the [Bernoulli inequality](../../../../../bernoulli-s-inequality.md), since $r^{-n}\ge1+n(r^{-1}-1)\to\infty$. Therefore the inner [limit](../../../../../limit-of-a-function.md) is

$$
\lim_{n\to\infty}\cos^{2n}(m!\pi x)=\begin{cases}1,&m!x\in\mathbb Z,\\0,&m!x\notin\mathbb Z.\end{cases}
$$

If $x=p/q$ is a [rational number](../../../../../rational-number.md), with $q\ge1$, then $q$ divides the [factorial](../../../../../factorial.md) $m!$ whenever $m\ge q$. Hence $m!x$ is an integer for all sufficiently large $m$, and the outer limit is one. This includes the endpoints $x=0,1$. If $x$ is an [irrational number](../../../../../irrational-number.md), $m!x$ cannot be an integer for any $m$, since division by $m!$ would make $x$ rational. Then every inner limit is zero. The [factorial cosine iterated limit detects rationality](../../../../../factorial-cosine-iterated-limit-detects-rationality.md) result is consequently

$$
\boxed{\lim_{m\to\infty}\left[\lim_{n\to\infty}\cos^{2n}(m!\pi x)\right]=\begin{cases}1,&x\in\mathbb Q,\\0,&x\notin\mathbb Q.\end{cases}}
$$

Each inner limit was taken with $m$ fixed; the argument does not interchange the two limits or assert a joint limit as both indices grow.

## ↑ Ancestors (10)

1. [9F](../9f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
