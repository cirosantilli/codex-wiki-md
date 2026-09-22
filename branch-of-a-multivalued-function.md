# Branch of a multivalued function

↑ **Parent:** [Branch point](branch-point.md)

A branch of a multivalued analytic expression is a single-valued [holomorphic function](holomorphic-function.md) on a specified domain that consistently selects one of the expression's possible values. A [branch cut](branch-cut.md) is a convenient way to choose such a domain, rather than an intrinsic locus of singularities. On $D=\mathbb C\setminus(-\infty,0]$, the [principal logarithm](principal-complex-logarithm.md) supplies two square-root branches

$$
B_+(z)=\exp\left(\tfrac12\operatorname{Log}z\right),\qquad B_-(z)=-B_+(z),\qquad B_\pm(z)^2=z.
$$

For $z=i$, these give $B_+(i)=e^{i\pi/4}=(1+i)/\sqrt2$ and $B_-(i)=-(1+i)/\sqrt2$. Their [derivatives](derivative.md) follow by differentiating $B_\pm^2=z$: $B_\pm'=1/(2B_\pm)$, so $B_+'(i)=(1-i)/(2\sqrt2)$. There are exactly two branches on $D$: for any other [holomorphic square root](holomorphic-square-root.md) $B$, the ratio $B/B_+$ is [continuous](continuous-function.md), takes values in $\{1,-1\}$, and hence is constant on the [connected](connected-space.md) domain.

The cut can move. Choosing $0<\theta<2\pi$ defines a [holomorphic logarithm](holomorphic-logarithm.md) $L_+(z)=\log|z|+i\theta$ on $D_+=\mathbb C\setminus[0,\infty)$. At $-1$ this gives $L_+(-1)=i\pi$ and $\exp(L_+(-1)/2)=i$, both regular values despite $-1$ lying on the previous cut. In the [complex upper half-plane](upper-half-plane-complex-analysis.md), $L_+$ agrees with $\operatorname{Log}$; in the [lower half-plane](lower-half-plane.md) it equals $\operatorname{Log}+2\pi i$, so the corresponding square roots have opposite signs there. The overlap $D\cap D_+$ has two components, exactly why the [identity theorem](identity-theorem.md) cannot force agreement between them. [Orloff, section 13.2.1, Example 13.4](https://ocw.mit.edu/courses/18-04-complex-variables-with-applications-spring-2018/af8c9c78c3915aaf3fd1695f8d32a3b3_MIT18_04S18_topic13.pdf)

For example, the limits of $B_+$ at $-r$, $r>0$, are $i\sqrt r$ from above and $-i\sqrt r$ from below. This jump records the chosen [branch cut](branch-cut.md); each point $-r\ne0$ still has a neighbourhood supporting a [holomorphic square root](holomorphic-square-root.md). Moving the cut changes the bookkeeping, while the [branch point](branch-point.md) at $0$ and its [monodromy](monodromy.md) persist. Specifying a [branch of a multivalued function](branch-of-a-multivalued-function.md) is therefore essential before differentiating or performing [contour integration](contour-integration.md) with [holomorphic square roots](holomorphic-square-root.md), [complex logarithms](complex-logarithm.md) or [complex exponentiation](complex-exponentiation.md).

## ↑ Ancestors (6)

1. [Branch point](branch-point.md)
2. [Complex analysis](complex-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Analytic continuation](analytic-continuation.md)
- [Argument (complex analysis)](argument-complex-analysis.md)
- [Branch of a multivalued function](branch-of-a-multivalued-function.md)
- [Holomorphic logarithm](holomorphic-logarithm.md)
- [Inverse tangent](inverse-tangent.md)
- [Monodromy](monodromy.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-1/13d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-50/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-50/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-3/4a/a/solution.md)
