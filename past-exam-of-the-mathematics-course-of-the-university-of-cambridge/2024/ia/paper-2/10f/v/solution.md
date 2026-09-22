<h1 id="10f/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Part (iii) and the given harmonic-sum asymptotic show that

$$
\frac{\mathbb ET_n}{n\log n}
=\frac{H_n}{\log n}\longrightarrow1.
$$

For any fixed $\varepsilon>0$, this deterministic ratio lies within $\varepsilon/2$ of $1$ for all sufficiently large $n$. The [Chebyshev inequality](../../../../../../chebyshev-inequality.md) and part (iv) then give

$$
\begin{aligned}
\mathbb P\left(
\left|\frac{T_n}{n\log n}-1\right|>\varepsilon
\right)
&\leq
\mathbb P\left(
|T_n-\mathbb ET_n|>\frac{\varepsilon}{2}n\log n
\right)\\
&\leq
\frac{4\operatorname{var}(T_n)}
{\varepsilon^2n^2(\log n)^2}\\
&\leq\frac{4C}{\varepsilon^2(\log n)^2}
\longrightarrow0.
\end{aligned}
$$

Thus

$$
\boxed{\frac{T_n}{n\log n}\longrightarrow1
\quad\hbox{in probability}.}
$$

## ↑ Ancestors (11)

1. [V](../v.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
