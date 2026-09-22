<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For metric signature $(+---)$, the momentum-space rules for the [Yukawa interaction](../../../../../yukawa-interaction.md) are:

- an internal scalar line contributes $i/(k^2-m_\phi^2+i\epsilon)$;
- an internal fermion contributes $i(\not k+m)/(k^2-m^2+i\epsilon)$;
- each $\phi\bar\psi\psi$ or $\phi\bar\chi\chi$ vertex contributes $-ig$;
- incoming and outgoing fermions contribute $u_r(p)$ and $\bar u_r(p)$, while incoming and outgoing antifermions contribute $\bar v_s(q)$ and $v_s(q)$;
- every closed fermion loop contributes an additional minus sign.

At leading order the process has one $s$-channel scalar propagator. With $s=(p+q)^2$,

$$
i\mathcal M
=\bigl[\bar v_s(q)(-ig)u_r(p)\bigr]
\frac{i}{s-m_\phi^2+i\epsilon}
\bigl[\bar u_{r'}(p')(-ig)v_{s'}(q')\bigr].
$$

Thus, up to an irrelevant overall sign,

$$
\mathcal M=-\frac{g^2}{s-m_\phi^2+i\epsilon}
[\bar v_s(q)u_r(p)][\bar u_{r'}(p')v_{s'}(q')].
$$

The [fermion spin sums](../../../../../fermion-spin-sum.md) and $\operatorname{tr}(\not a\not b)=4a\mathbin\cdot b$ give

$$
\sum_{r,s}|\bar v_s(q)u_r(p)|^2=4(p\mathbin\cdot q-m_\psi^2),
$$

and the analogous final sum is $4(p'\mathbin\cdot q'-m_\chi^2)$. Therefore

$$
X=\frac{4g^4(p\mathbin\cdot q-m_\psi^2)
(p'\mathbin\cdot q'-m_\chi^2)}{(s-m_\phi^2)^2}.
$$

Using $p\mathbin\cdot q=(s-2m_\psi^2)/2$ and its final-state analogue yields

$$
\boxed{X=\frac{g^4(s-4m_\psi^2)(s-4m_\chi^2)}{(s-m_\phi^2)^2}}.
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 301](../../paper-301-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
