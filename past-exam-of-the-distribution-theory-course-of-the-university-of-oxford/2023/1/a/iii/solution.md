<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

On each interval $[k,k+1]$, $k\in\mathbb Z$, the [function](../../../../../function-split.md) is $d(x)=x-k$ on $[k,k+\tfrac12]$ and $d(x)=k+1-x$ on $[k+\tfrac12,k+1]$. Its ordinary [derivative](../../../../../derivative.md) exists off $\tfrac12\mathbb Z$ and is the [locally integrable function](../../../../../locally-integrable-function.md)

$$
s(x)=\begin{cases}
1,&k<x<k+\tfrac12,\\
-1,&k+\tfrac12<x<k+1,
\end{cases}\qquad k\in\mathbb Z.
$$

Assign arbitrary values at the endpoints. For a [test function](../../../../../test-function.md) $\phi$, split $-\int d\phi'$ at these corners and apply [integration by parts](../../../../../integration-by-parts.md) on each piece. The adjacent [boundary terms](../../../../../boundary-term.md) cancel because $d$ is continuous, and only finitely many pieces meet the [compact support](../../../../../compact-support.md) of $\phi$. Hence

$$
\boxed{\langle d',\phi\rangle=\int_{\mathbb R}s(x)\phi(x)\,dx,\qquad d'=s.}
$$

The [distributional derivative](../../../../../distributional-derivative.md) is exactly the [regular distribution](../../../../../regular-distribution.md) of the ordinary [derivative](../../../../../derivative.md) defined [almost everywhere](../../../../../almost-everywhere.md). There are no [Dirac delta distributions](../../../../../dirac-delta-function.md) in this first [distributional derivative](../../../../../distributional-derivative.md): corners change slope, while a jump of the [function](../../../../../function-split.md) itself would create a point mass.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the distribution theory course of the University of Oxford](../../../../split.md)
6. [Distribution theory course of the University of Oxford](../../../../../distribution-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
