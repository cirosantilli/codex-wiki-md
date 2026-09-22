<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Beurling–Gelfand spectral radius formula](../../../../../../spectral-radius-formula.md) states that for every element $a$ of a complex [Banach algebra](../../../../../../banach-algebra-split.md),

$$
\boxed{r(a)=\max_{\lambda\in\sigma(a)}|\lambda|
=\lim_{n\to\infty}\|a^n\|^{1/n}=\inf_{n\geq1}\|a^n\|^{1/n}.}
$$

For a [Hermitian element of a C-star algebra](../../../../../../hermitian-element-of-a-c-star-algebra.md) $a=a^*$, the [C-star identity](../../../../../../c-star-identity.md) gives $\|a^2\|=\|a\|^2$. Iterating,

$$
\|a^{2^m}\|=\|a\|^{2^m}.
$$

The subsequence $n=2^m$ in the spectral-radius limit therefore proves $\boxed{r(a)=\|a\|}$.

Let $\theta:A\to B$ be a unital [C-star homomorphism](../../../../../../c-star-homomorphism.md). If $a-\lambda1$ is invertible in $A$, its inverse is sent to an inverse of $\theta(a)-\lambda1$ in $B$. Thus $\sigma_B(\theta(a))\subseteq\sigma_A(a)$ without assuming continuity of $\theta$. For Hermitian $a$, $\theta(a)$ is also Hermitian, so

$$
\|\theta(a)\|=r_B(\theta(a))\leq r_A(a)=\|a\|.
$$

For arbitrary $x\in A$, apply this inequality to $x^*x$ and the [C-star identity](../../../../../../c-star-identity.md) in both algebras:

$$
\|\theta(x)\|^2=\|\theta(x)^*\theta(x)\|=\|\theta(x^*x)\|\leq\|x^*x\|=\|x\|^2.
$$

Hence $\boxed{\|\theta(x)\|\leq\|x\|}$ for every $x$.

Now assume $\theta$ is injective. For a fixed $x$, it is enough to prove norm preservation on $C=C^*(1,x^*x)$, a commutative unital [C-star algebra](../../../../../../c-star-algebra.md): the preceding square-norm identity will then recover the norm of $x$. By the [Commutative Gelfand--Naimark theorem](../../../../../../commutative-gelfand-naimark-theorem.md), identify $C$ with $C(K)$. Let $D=\overline{\theta(C)}\subseteq B$. It is also a commutative unital [C-star algebra](../../../../../../c-star-algebra.md), and its [character space](../../../../../../character-space-of-an-algebra.md) $\Phi_D$ is compact. Each $\chi\in\Phi_D$ restricts along $\theta$ to a character of $C(K)$, hence to evaluation at a point $q(\chi)\in K$. The map $q:\Phi_D\to K$ is continuous, so $L=q(\Phi_D)$ is closed.

If $L\ne K$, the [Urysohn lemma](../../../../../../urysohn-s-lemma.md) provides a nonzero $f\in C(K)$ vanishing on $L$. Then $\chi(\theta(f))=f(q(\chi))=0$ for every $\chi\in\Phi_D$. Faithfulness of the [Gelfand transform](../../../../../../gelfand-representation.md) in $D$ gives $\theta(f)=0$, contradicting injectivity. Thus $q$ is onto. The isometric [Gelfand transform](../../../../../../gelfand-representation.md) of $D$ now gives

$$
\|\theta(f)\|=\sup_{\chi\in\Phi_D}|\chi(\theta(f))|
=\sup_{t\in K}|f(t)|=\|f\|\quad(f\in C).
$$

Finally,

$$
\|\theta(x)\|^2=\|\theta(x^*x)\|=\|x^*x\|=\|x\|^2,
\qquad\boxed{\|\theta(x)\|=\|x\|.}
$$

This proves that an [injective C-star homomorphism is isometric](../../../../../../injective-c-star-homomorphism-is-isometric.md) without assuming its image is closed before norm preservation has been established.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
