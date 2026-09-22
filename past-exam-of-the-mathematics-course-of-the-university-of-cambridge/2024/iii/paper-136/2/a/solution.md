<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a finite extension $L/K$ of [local fields](../../../../../../local-field.md), let $e=e(L/K)$ be its [ramification index](../../../../../../ramification-index.md) and $f=f(L/K)=[k_L:k_K]$ its [residue-field degree](../../../../../../residue-field-degree.md). An [unramified extension](../../../../../../unramified-extension.md) has $e=1$. A [totally ramified extension](../../../../../../totally-ramified-extension.md) has $e=[L:K]$, equivalently $f=1$. A [tamely ramified extension](../../../../../../tamely-ramified-extension.md) has separable residue extension and ramification index coprime to the residue characteristic.

Let $\bar\theta$ generate the finite extension $k_L/k_K$, and let $\bar g$ be its [minimal polynomial](../../../../../../minimal-polynomial.md). Lift $\bar g$ to a monic $g\in\mathcal O_K[X]$ and choose any lift $t\in\mathcal O_L$ of $\bar\theta$. Since finite fields are [perfect fields](../../../../../../perfect-field.md), $\bar g'(\bar\theta)\ne0$. The simple-root form of [Hensel lemma](../../../../../../hensel-s-lemma.md), applied inside $L$, gives $\theta\in\mathcal O_L$ with

$$
g(\theta)=0,
\qquad \theta\equiv t\pmod{\mathfrak m_L}.
$$

Set $K_0=K(\theta)$. Its residue field contains $k_K(\bar\theta)=k_L$, so

$$
[K_0:K]\geq[k_L:k_K]=f.
$$

The equation $g(\theta)=0$ gives the reverse inequality. Thus $[K_0:K]=f$, its residue-field degree is $f$, and $e(K_0/K)=1$; hence $K_0/K$ is unramified. Since $k_{K_0}=k_L$, the extension $L/K_0$ has residue-field degree one and is totally ramified. This constructs the [maximal unramified subextension of a local field extension](../../../../../../maximal-unramified-subextension-of-a-local-field-extension.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
