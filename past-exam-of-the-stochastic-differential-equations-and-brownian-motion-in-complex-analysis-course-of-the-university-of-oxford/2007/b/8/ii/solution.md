<h1 id="b/8/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Using the [Cauchy distribution](../../../../../cauchy-distribution.md) from the preceding part gives one common [probability space](../../../../../probability-space-split.md) for all starting points:

$$
\phi(x+iy)=\mathbb E[f(x+yC)]\quad(y>0).
$$

As $(x,y)\to(0,0)$ with $y>0$, $x+yC\to0$ almost surely, since $C$ is a finite real [random variable](../../../../../random-variable-split.md) almost surely. [Continuity](../../../../../continuous-function.md) of $f$ at zero gives $f(x+yC)\to f(0)$ almost surely, and boundedness supplies an integrable constant bound. [Dominated convergence theorem](../../../../../dominated-convergence-theorem.md) therefore proves

$$
\boxed{\lim_{\substack{z\to0\\\Im z>0}}\phi(z)=f(0)=\phi(0).}
$$

The argument applies to every sequence approaching zero, including tangential approaches. Along the real boundary the extension is already $f$, which is continuous. Hence the extension is **continuous at zero in the closed half-plane**. No finite moment of the [Cauchy distribution](../../../../../cauchy-distribution.md) is required.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
