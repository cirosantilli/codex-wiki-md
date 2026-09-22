# Little o notation

↑ **Parent:** [Big O notation](big-o-notation.md)

When $g$ is nonzero sufficiently near the specified [limit](limit-of-a-function.md), little o notation means

$$
\boxed{f=o(g)\quad\Longleftrightarrow\quad f/g\longrightarrow0.}
$$

Thus the numerator becomes negligible relative to the denominator's scale. As $n\to\infty$, $n=o(n^2)$ because $n/n^2=1/n\to0$; as $h\to0$, $h^2=o(h)$ because $h^2/h=h\to0$. The direction of the [limit](limit-of-a-function.md) changes the comparison. [MIT Mathematics for Computer Science, §9.7.1: little-oh comparison](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-fall-2010/93cad640cf3ed0b23ef70688f452d4d5_MIT6_042JF10_notes.pdf#page=281)

Equivalently, for every $\varepsilon>0$, the bound $|f|\le\varepsilon|g|$ holds sufficiently near that [limit](limit-of-a-function.md), with a threshold allowed to depend on $\varepsilon$. [Big O notation](big-o-notation.md) needs only one fixed multiplier, making it weaker. For example, $2n=O(n)$ but $2n$ is not $o(n)$. The useful relation $f\sim g\Longleftrightarrow f-g=o(g)$ turns [asymptotic equivalence](asymptotic-equivalence.md) into a statement about a negligible remainder.

## ↑ Ancestors (6)

1. [Big O notation](big-o-notation.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Asymptotic analysis](asymptotic-analysis.md)
- [Asymptotic comparison of exponential functions](asymptotic-comparison-of-exponential-functions.md)
- [Asymptotic equivalence](asymptotic-equivalence.md)
