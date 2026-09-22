# Extinction probability of a branching process

↑ **Parent:** [Galton-Watson extinction fixed point](galton-watson-extinction-fixed-point.md)

For a [Galton-Watson process](galton-watson-process.md) with one ancestor, the [branching extinction probability](extinction-probability-of-a-branching-process.md) is the [probability](probability.md) that some generation is empty:

$$
q=\mathbb P\left(\bigcup_{n\geq0}\{Z_n=0\}\right)=\lim_{n\to\infty}\mathbb P(Z_n=0).
$$

The equality uses the [absorbing state](absorbing-state.md) at zero. The complementary [branching survival probability](survival-probability-of-a-branching-process.md) $1-q$ is the [probability](probability.md) that every generation is nonempty. The [Galton-Watson extinction fixed point](galton-watson-extinction-fixed-point.md) computes $q$ from the [offspring distribution](offspring-distribution-of-a-branching-process.md).

For $p_0=p_1=1/4$, $p_2=1/2$, one ancestor has $q=1/2$. Starting instead from $m$ ancestors with [independent](independent-random-variables.md) descendant families gives

$$
\mathbb P(\text{eventual extinction}\mid Z_0=m)=q^m,\qquad \mathbb P(Z_n=0\mid Z_0=m)=q_n^m.
$$

All $m$ families must die out. With three ancestors, eventual extinction has [probability](probability.md) $1/8$ and survival has [probability](probability.md) $7/8$; by generation two, extinction has [probability](probability.md) $(11/32)^3=1331/32768\approx0.040619$. Extra ancestors change the extinction [probability](probability.md) without changing the [offspring distribution](offspring-distribution-of-a-branching-process.md). [University of Münster branching-process notes, Lemma 1.2 and equation (1.10)](https://www.uni-muenster.de/Stochastik/lehre/WS1011/SpezielleStochastischeProzesse/Ch_1.pdf)

For finite offspring [mean](expected-value.md) $\mu$, the extinction classification is:
- If $\mu<1$, extinction has [probability](probability.md) $1$. For example $p_0=3/4$, $p_2=1/4$ gives $\mu=1/2$ and $F(s)=3/4+s^2/4$; its only [fixed point](fixed-point.md) in $[0,1]$ is $1$.
- If $\mu=1$ and $p_1\ne1$, extinction also has [probability](probability.md) $1$. For example $p_0=p_2=1/2$ gives $F(s)-s=(s-1)^2/2$ and $q=1$, despite [expected generation size in a Galton-Watson process](expected-generation-size-in-a-galton-watson-process.md) remaining one.
- If $1<\mu<\infty$, extinction has [probability](probability.md) $q<1$. The value can be zero: if $p_0=0$, every individual has at least one child, so an initially nonempty family never becomes empty. In particular $p_2=1$ gives $Z_n=2^n$ and $q=0$.

The critical exception is $p_1=1$: every individual has exactly one child, $F(s)=s$, and $Z_n=1$ forever from one ancestor. Thus $\mu=1$ but $q=0$; a blanket claim that every critical [Galton-Watson process](galton-watson-process.md) becomes extinct would be false. These cases concern the [Galton-Watson process](galton-watson-process.md) with its common [offspring distribution](offspring-distribution-of-a-branching-process.md) and [independence](independent-random-variables.md) assumptions. [University of Münster branching-process notes, Section 1.4, trivial cases and Theorem 1.7](https://www.uni-muenster.de/Stochastik/lehre/WS1011/SpezielleStochastischeProzesse/Ch_1.pdf)

This [probability](probability.md) answers whether any lineage persists, which the offspring [mean](expected-value.md) alone cannot quantify in the supercritical case. A [branching process conditioned on extinction](branching-process-conditioned-on-extinction.md) uses the same [fixed point](fixed-point.md) to reweight reproduction and describe families known eventually to die out.

**Table of contents**

- [Survival probability of a branching process](survival-probability-of-a-branching-process.md)

## ↑ Ancestors (6)

1. [Galton-Watson extinction fixed point](galton-watson-extinction-fixed-point.md)
2. [Galton-Watson process](galton-watson-process.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Laziness invariance of branching extinction](laziness-invariance-of-branching-extinction.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-2/11f/solution.md)
