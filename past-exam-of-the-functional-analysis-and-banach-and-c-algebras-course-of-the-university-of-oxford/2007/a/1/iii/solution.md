<h1 id="a/1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Since the kernel has integral one, The [Tonelli theorem](../../../../../tonelli-theorem.md) and the [triangle inequality](../../../../../triangle-inequality.md) give

$$
\|f*g-f\|_1\leq\int g(s)\left(\int|f(t-s)-f(t)|dt\right)ds\leq\sup_{|h|\leq\delta}\|f(\cdot+h)-f\|_1.
$$

This proves **the stated [convolution](../../../../../convolution.md) approximation estimate**.

For the unlabelled compactness assertion let $M$ bound the [norms](../../../../../norm.md) of $S$, and fix $\eta>0$. Choose the kernel width $\delta$ smaller than the translation radius supplied for $\eta$, so that the same bound holds for all shifts of size at most this width. The preceding estimate gives $\|f*g-f\|_1<\eta$ uniformly. The smoothed family has uniform bound $M/\delta$ and uniform Lipschitz constant $M/\delta^2$. Choose $K$ with all original tails outside $[-K,K]$ below $\eta$, and put $L=K+\delta$. The [Tonelli theorem](../../../../../tonelli-theorem.md) gives

$$
\int_{|t|\geq L}|(f*g)(t)|dt\leq\int g(s)\int_{|u|\geq K}|f(u)|du\,ds<\eta.
$$

On $[-L,L]$ the smoothed family is relatively compact in the uniform [norm](../../../../../norm.md) by the [Arzelà-Ascoli theorem](../../../../../arzela-ascoli-theorem.md). Take a finite uniform net with error below $\eta/(2L)$ and extend its centers by zero outside that interval. It is a finite $L^1$ net for the smoothed-and-truncated family with error $\eta$. Each original $f$ is within another $2\eta$ of its corresponding truncated smoothing. Thus **$S$ is [totally bounded](../../../../../totally-bounded-space.md) in $L^1$**. The displayed (a),(b) are the two hypotheses used together in this argument.

For the final family, [Young convolution inequality](../../../../../young-s-convolution-inequality.md) gives $\|f_0*f\|_1\leq\|f_0\|_1$. Its translations satisfy

$$
\|\tau_h(f_0*f)-f_0*f\|_1\leq\|\tau_hf_0-f_0\|_1\|f\|_1\leq\|\tau_hf_0-f_0\|_1,
$$

which tends to zero uniformly over the family. Since $f$ vanishes outside $[-1,1]$,

$$
\int_{|t|\geq K}|(f_0*f)(t)|dt\leq\|f\|_1\int_{|u|\geq K-1}|f_0(u)|du\longrightarrow0
$$

uniformly as well. Both compactness hypotheses apply, proving **$S_0$ is [totally bounded](../../../../../totally-bounded-space.md)**.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../split.md)
6. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
