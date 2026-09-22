<h1 id="b/8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\lambda=a+ib$ with $b\ne0$. Since $aI-T$ is self-adjoint, $\langle(aI-T)v,v\rangle$ is real. The cross term in the squared [norm](../../../../../norm.md) therefore vanishes:

$$
\|(\lambda I-T)v\|^2=\|(aI-T)v\|^2+b^2\|v\|^2=\|(\overline\lambda I-T)v\|^2.
$$

This proves the equality and lower bound, and makes both $S=\lambda I-T$ and $S^*=\overline\lambda I-T$ [injective](../../../../../injective-function.md).

If $Sv_n$ converges, the lower bound shows $v_n$ is Cauchy. [Completeness](../../../../../completeness.md) gives $v_n\to v$ and boundedness gives $Sv_n\to Sv$, so the range is closed. Also $(\operatorname{ran}S)^\perp=\ker S^*=0$, so the range is [dense](../../../../../dense-set.md). Being both closed and [dense](../../../../../dense-set.md), it equals $V$. Hence $S$ is bijective, and its lower bound gives

$$
\boxed{\|(\lambda I-T)^{-1}\|\leq|\operatorname{Im}\lambda|^{-1},\qquad\sigma(T)\subseteq\mathbb R.}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the analysis course of the University of Oxford](../../../../split.md)
6. [Analysis course of the University of Oxford](../../../../../analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
