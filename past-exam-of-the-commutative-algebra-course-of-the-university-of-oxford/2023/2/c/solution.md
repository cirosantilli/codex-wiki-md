<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $n\geq1$, let $K_n=\ker(\phi^n)$, where the power denotes repeated composition of the [ring endomorphism](../../../../ring-endomorphism.md). These [ideals](../../../../ideal.md) form an ascending chain:

$$
K_1\subseteq K_2\subseteq K_3\subseteq\cdots.
$$

The [ascending chain condition](../../../../ascending-chain-condition.md) for a [Noetherian ring](../../../../noetherian-ring.md) gives $K_N=K_{N+1}$ for some $N\geq1$. Take $a\in\ker\phi$. Since $\phi$ is [surjective](../../../../surjective-function.md), its iterate $\phi^N$ is [surjective](../../../../surjective-function.md), so choose $b\in R$ with $\phi^N(b)=a$. Then

$$
\phi^{N+1}(b)=\phi(a)=0,
$$

so $b\in K_{N+1}=K_N$. Therefore $a=\phi^N(b)=0$.

Thus the [kernel of a ring homomorphism](../../../../kernel-of-a-ring-homomorphism.md) $\phi$ is zero. This proves that a [surjective endomorphism of a Noetherian ring is an automorphism](../../../../surjective-endomorphism-of-a-noetherian-ring-is-an-automorphism.md), and in particular

$$
\boxed{\phi\text{ is injective}.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the commutative algebra course of the University of Oxford](../../../split.md)
5. [Commutative algebra course of the University of Oxford](../../../../commutative-algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
