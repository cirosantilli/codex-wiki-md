<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $X=\operatorname{Spec}R$ be an [affine scheme](../../../../affine-scheme.md), and let $(U_\lambda)_{\lambda\in\Lambda}$ be an [open cover](../../../../open-cover.md). Write each complement as a [Zariski closed](../../../../zariski-closed-set.md) subset $X\setminus U_\lambda=V(I_\lambda)$ for an [ideal](../../../../ideal.md) $I_\lambda\subseteq R$. The intersection rule for [Zariski closed](../../../../zariski-closed-set.md) subsets gives

$$
\varnothing=\bigcap_{\lambda\in\Lambda}V(I_\lambda)
=V\!\left(\sum_{\lambda\in\Lambda}I_\lambda\right).
$$

A proper [ideal](../../../../ideal.md) lies in a [maximal ideal](../../../../maximal-ideal.md), which is a [prime ideal](../../../../prime-ideal.md); consequently $V(J)=\varnothing$ forces $J=R$. Thus $1\in\sum_\lambda I_\lambda$. By the definition of a sum of [ideals](../../../../ideal.md), this membership is witnessed by finitely many elements:

$$
1=a_1+\cdots+a_r,\qquad a_j\in I_{\lambda_j}.
$$

Hence $\sum_{j=1}^r I_{\lambda_j}=R$, so $\bigcap_{j=1}^r V(I_{\lambda_j})=\varnothing$, and therefore $X=\bigcup_{j=1}^r U_{\lambda_j}$. If $R$ is the [zero ring](../../../../zero-ring.md), $X$ is empty and the empty subcover suffices. This proves

$$
\boxed{\text{Every affine scheme is quasi-compact}.}
$$

The proof uses only complements, the intersection rule for [Zariski closed](../../../../zariski-closed-set.md) subsets, and the finite expression of an element in a sum of [ideals](../../../../ideal.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the introduction to schemes course of the University of Oxford](../../../split.md)
5. [Introduction to schemes course of the University of Oxford](../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
