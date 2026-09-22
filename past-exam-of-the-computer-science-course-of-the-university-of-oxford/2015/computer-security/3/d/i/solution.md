<h1 id="3/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For authenticate-then-encrypt, write the intercepted pair as $(c,t)=(E_k(x),E_k(s))$, where $s=f(\mathit{sk},x)$. Each trial key $k'$ gives

$$
x'=D_{k'}(c),\qquad s'=D_{k'}(t).
$$

The adversary can check the public relation

$$
\boxed{g(\mathit{pk},s')\stackrel{?}=x'.}
$$

The true key always passes. An incorrect key will generally fail, and further intercepted pairs can eliminate accidental matches. This gives a [ciphertext-only attack](../../../../../../ciphertext-only-attack.md) with a useful key-testing predicate even when the [plaintext](../../../../../../plaintext.md) has no recognisable format. It makes [exhaustive key search](../../../../../../exhaustive-key-search.md) applicable with less prior information; it does not reduce the generic key-space size below $2^m$.

The usual approximate false-pass chance $2^{-n}$ is an ideal-behaviour estimate, not a consequence of the bare permutation identities alone. The decisive point is that the encrypted [digital signature](../../../../../../digital-signature.md) supplies publicly checkable redundancy once a candidate [decryption](../../../../../../decryption.md) key is tried.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Computer security](../../../../computer-security-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
