# Rational polynomial content

↑ **Parent:** [Polynomial content](polynomial-content.md)

For a nonzero [polynomial](polynomial-split.md) $g\in\mathbb Q[t]$, choose a positive [integer](integer-split.md) $n$ clearing its denominators and set $c(g)=c(ng)/n$, where the [polynomial content](polynomial-content.md) of an integer-coefficient [polynomial](polynomial-split.md) is the positive [greatest common divisor](greatest-common-divisor.md) of its coefficients. This is independent of $n$: if $f/n=h/m$, then $mf=nh$, hence $mc(f)=nc(h)$.

The integer-coefficient product formula from [Gauss lemma for polynomials](gauss-lemma-for-polynomials.md) gives

$$
c(g_1g_2)=c(g_1)c(g_2),\qquad
c(rg)=|r|c(g)\quad(r\in\mathbb Q\setminus\{0\}).
$$

Moreover $g/c(g)$ is an integer-coefficient [primitive polynomial](primitive-polynomial.md): if $g=f/n$, then $g/c(g)=f/c(f)$. For example,

$$
g(t)=\frac23t^2-\frac49t+\frac29
\quad\Longrightarrow\quad
c(g)=\frac29,\qquad g/c(g)=3t^2-2t+1.
$$

This normalization proves a useful divisibility descent. If $f\in\mathbb Z[t]$ is [primitive](primitive-polynomial.md), $g\in\mathbb Z[t]$ and $g=fq$ for $q\in\mathbb Q[t]$, then $c(q)=c(g)$ is an [integer](integer-split.md). Since $q/c(q)\in\mathbb Z[t]$, it follows that $q\in\mathbb Z[t]$.

## ↑ Ancestors (6)

1. [Polynomial content](polynomial-content.md)
2. [Commutative algebra](commutative-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-algebra-2-course-of-the-university-of-oxford/2014/2/a/solution.md)
- [Solution](past-exam-of-the-algebra-2-course-of-the-university-of-oxford/2015/3/a/solution.md)
- [Solution](past-exam-of-the-algebra-2-course-of-the-university-of-oxford/2015/3/c/solution.md)
- [Prime ideals of the integer polynomial ring above zero](prime-ideals-of-the-integer-polynomial-ring-above-zero.md)
