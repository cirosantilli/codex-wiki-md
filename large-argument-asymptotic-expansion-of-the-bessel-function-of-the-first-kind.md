# Large-argument asymptotic expansion of the Bessel function of the first kind

↑ **Parent:** [Bessel function of the first kind](bessel-function-of-the-first-kind.md)

For fixed $\nu$, put

$$
\chi=z-\frac{\pi\nu}{2}-\frac\pi4,
\qquad
a_k(\nu)=\frac{\prod_{j=1}^k\left(4\nu^2-(2j-1)^2\right)}{k!8^k},
\qquad a_0=1.
$$

Then

$$
J_\nu(z)\sim\sqrt{\frac2{\pi z}}
\left[
\cos\chi\sum_{m=0}^{\infty}\frac{(-1)^ma_{2m}(\nu)}{z^{2m}}
-\sin\chi\sum_{m=0}^{\infty}\frac{(-1)^ma_{2m+1}(\nu)}{z^{2m+1}}
\right]
$$

as $|z|\to\infty$, uniformly for $|\arg z|\leq\pi-\delta$. In particular,

$$
J_\nu(z)\sim\sqrt{\frac2{\pi z}}
\left[
\cos\chi-\frac{4\nu^2-1}{8z}\sin\chi
-\frac{(4\nu^2-1)(4\nu^2-9)}{2!(8z)^2}\cos\chi+\cdots
\right].
$$

## ↑ Ancestors (6)

1. [Bessel function of the first kind](bessel-function-of-the-first-kind.md)
2. [Bessel function](bessel-function.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-41/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-74/1/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/30a/b/solution.md)
