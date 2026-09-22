<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

Fix $z_0\in E$ and $\epsilon>0$. Choose $N$ so that $\sup_E|f_N-f|<\epsilon/3$, and then choose $\delta>0$ so that $|f_N(z)-f_N(z_0)|<\epsilon/3$ for $z\in E$ with $|z-z_0|<\delta$. The [triangle inequality](../../../../../triangle-inequality.md) gives $|f(z)-f(z_0)|<\epsilon$. This proves the [uniform limit theorem](../../../../../uniform-limit-theorem.md) on the relative topology of $E$, whether or not $E$ is open.

The [Weierstrass M-test](../../../../../weierstrass-m-test.md) states that if $|u_n(z)|\le M_n$ for every $z\in E$ and $\sum M_n<\infty$, then $\sum u_n$ converges uniformly and absolutely on $E$. Indeed, the supremum of a tail is at most the corresponding tail of $\sum M_n$, proving the uniform Cauchy criterion.

For the given [secant function](../../../../../secant-trigonometry.md) terms, a denominator can vanish only at $z=n(2k+1)$, an integer. Thus every individual term is continuous off the integers. Fix $z_0\notin\mathbb Z$, and choose a closed [disk](../../../../../disk-mathematics.md) $K$ about $z_0$ containing no integer. Let $R=\sup_K|\operatorname{Re}z|$ and take $N>2R$. For $n\ge N$, $|\pi\operatorname{Re}z/(2n)|<\pi/4$; the permitted cosine inequality gives

$$
\left|n^{-2}\sec\frac{\pi z}{2n}\right|\le\frac{\sqrt2}{n^2}\quad(z\in K).
$$

The [Weierstrass M-test](../../../../../weierstrass-m-test.md) makes the tail uniformly convergent on $K$. The finitely many earlier terms are continuous there, so the [uniform limit theorem](../../../../../uniform-limit-theorem.md) makes their sum continuous at $z_0$. Therefore **$f$ is continuous on $\mathbb C\setminus\mathbb Z$**. The argument is local; a global M-test on the whole punctured plane would fail near its [poles](../../../../../pole.md).

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
