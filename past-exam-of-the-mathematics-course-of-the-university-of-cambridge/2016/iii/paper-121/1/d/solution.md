<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**Yes.** A [cardinal fixed point of the singular cardinal enumeration](../../../../../../cardinal-fixed-point-of-the-singular-cardinal-enumeration.md) is obtained by countable iteration. Start with $\kappa_0=\aleph_0$ and put

$$
\kappa_{n+1}=\sigma_{\kappa_n}.
$$

The [singular cardinal enumeration](../../../../../../singular-cardinal-enumeration.md) is strictly increasing and satisfies $\sigma_\alpha\geq\alpha$ for every [ordinal](../../../../../../ordinal.md) $\alpha$; the latter follows by [transfinite induction](../../../../../../transfinite-induction.md) for any strictly increasing ordinal-valued enumeration. If equality occurs at some $\kappa_n$, that [cardinal number](../../../../../../cardinal-number.md) is already a witness. Otherwise the sequence is strictly increasing. Put $\kappa=\sup_{n<\omega}\kappa_n$. This is an uncountable [singular cardinal](../../../../../../singular-cardinal.md) of [cofinality](../../../../../../cofinality.md) $\omega$.

For every $\alpha<\kappa$, some $n$ has $\alpha<\kappa_n$, and therefore

$$
\sigma_\alpha<\sigma_{\kappa_n}=\kappa_{n+1}<\kappa.
$$

Also $\sup_n\sigma_{\kappa_n}=\kappa$, so $\sup_{\alpha<\kappa}\sigma_\alpha=\kappa$. At a [limit ordinal](../../../../../../limit-ordinal.md) index, if the supremum of all preceding enumerated cardinals is itself singular, it is exactly the next member: every smaller singular cardinal already has a preceding index. Thus

$$
\boxed{\sigma_\kappa=\kappa}.
$$

This argument uses continuity only at a singular supremum; the enumeration need not be continuous at a [weakly inaccessible cardinal](../../../../../../weakly-inaccessible-cardinal.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
