# Galton-Watson extinction fixed point

↑ **Parent:** [Galton-Watson process](galton-watson-process.md)

For a [Galton-Watson process](galton-watson-process.md) with one ancestor and offspring [probability generating function](probability-generating-function.md) $F$, the [branching extinction probability](extinction-probability-of-a-branching-process.md) $q$ is the smallest [fixed point](fixed-point.md) of $F$ in $[0,1]$. A direct way to find it is to compute extinction by generation $n$:

$$
q_0=0,\qquad q_n=\mathbb P(Z_n=0),\qquad q_{n+1}=F(q_n),\qquad q_n\uparrow q.
$$

Zero is an [absorbing state](absorbing-state.md), so extinction by generation $n$ is exactly the [event](event.md) $Z_n=0$. [Hao Wu, MIT 18.445, Lecture 19, slide 4](https://ocw.mit.edu/courses/18-445-introduction-to-stochastic-processes-spring-2015/27aaeb9eb9a9cecce93d9ad74413ddf5_MIT18_445S15_lecture19.pdf)

For $F(s)=1/4+s/4+s^2/2$, the equation is

$$
F(s)-s=\frac12\left(s-\frac12\right)(s-1)=0.
$$

Both $1/2$ and $1$ are [fixed points](fixed-point.md), but iteration from zero selects $q=1/2$. The first values are $q_1=1/4$, $q_2=11/32$, $q_3=809/2048\approx0.395020$, and $q_6\approx0.462186$. Iteration started at $1$ would stay at $1$ forever and would give the wrong extinction answer for this [offspring distribution](offspring-distribution-of-a-branching-process.md).

<a id="image-the-smallest-extinction-fixed-point-selected-by-iteration-from-zero"></a>
![](branching-extinction-fixed-point.png)

**[Figure 12](#image-the-smallest-extinction-fixed-point-selected-by-iteration-from-zero). The smallest extinction fixed point selected by iteration from zero**.

The vertical steps in the figure apply the offspring [probability generating function](probability-generating-function.md); horizontal steps return to the diagonal to start the next iteration. This gives a useful numerical calculation even when solving $F(s)=s$ explicitly is difficult. For the displayed law, every finite iteration is a lower bound for the eventual [branching extinction probability](extinction-probability-of-a-branching-process.md); at generation six, about $0.037814$ additional extinction [probability](probability.md) remains beyond the current empty families.

Why the smallest [fixed point](fixed-point.md)? The ancestor's children's descendant families are [independent](independent-random-variables.md); given $k$ children, all are empty $n$ generations later with [probability](probability.md) $q_n^k$. Averaging gives $q_{n+1}=\sum_kp_kq_n^k=F(q_n)$. The increasing extinction [events](event.md) give the [limit](limit-of-a-function.md) $q$, and [continuity](continuous-function.md) of the [probability generating function](probability-generating-function.md) yields $F(q)=q$. For any other [fixed point](fixed-point.md) $r\in[0,1]$, $q_0\leq r$ and [monotonicity](monotonic-function.md) of $F$ imply $q_n\leq r$ at every step; hence $q\leq r$. [University of Münster branching-process notes, Section 1.4, Theorem 1.7](https://www.uni-muenster.de/Stochastik/lehre/WS1011/SpezielleStochastischeProzesse/Ch_1.pdf)

**Table of contents**

- [Laziness invariance of branching extinction](laziness-invariance-of-branching-extinction.md)
- [Extinction probability of a branching process](extinction-probability-of-a-branching-process.md)
  - [Survival probability of a branching process](survival-probability-of-a-branching-process.md)

## ↑ Ancestors (5)

1. [Galton-Watson process](galton-watson-process.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Extinction probability of a branching process](extinction-probability-of-a-branching-process.md)
- [Galton-Watson process](galton-watson-process.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-2/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-2/10f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-2/11f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-2/11f/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ia/paper-1/4f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-2/12f/b/solution.md)
