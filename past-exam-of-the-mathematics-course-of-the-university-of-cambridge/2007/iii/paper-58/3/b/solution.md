<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The PDF places the extra $X$ on $q_2$ after that qubit has interacted with $a_1$ but before it interacts with $a_2$. Its timing is essential. With no incoming error, the first extracted parity is zero. The fault then changes the data to

$$
u|010\rangle+v|101\rangle.
$$

The remaining parity measurement gives $a_2=1$ on both branches. Thus the measured [error syndrome](../../../../../../error-syndrome.md) is $01$, which the rule in the preceding part interprets as an error on $q_1$. Applying $X_1$ leaves

$$
\boxed{u|110\rangle+v|001\rangle=X_1X_2|\psi_L\rangle.}
$$

This is outside the original encoded subspace: neither of its supporting basis strings is $000$ or $111$. The incorrect syndrome causes a second data error rather than restoring the input. This [timed bit flip during repetition-code syndrome extraction](../../../../../../timed-bit-flip-during-repetition-code-syndrome-extraction.md) demonstrates why a simple parity circuit need not tolerate its own faults.

The same failure can be checked for every incoming channel error. Let $f\in\{0,1\}$ indicate the internal fault and let $c(s)$ be the correction bit pattern from the table. The observed syndrome and the final pre-correction data pattern are

$$
s_{\mathrm{obs}}=s(e)\oplus(0,f),\qquad d=e\oplus(0,f,0).
$$

Because $s$ is linear over binary addition and $s(c(s_{\mathrm{obs}}))=s_{\mathrm{obs}}$, the residual pattern $r=d\oplus c(s_{\mathrm{obs}})$ satisfies

$$
\boxed{s(r)=s(d)\oplus s_{\mathrm{obs}}=(f,0).}
$$

Whenever the fault occurs, the residual syndrome is $10$, so recovery never returns the state to the encoded subspace, even if a channel error also occurred. The diagram therefore must not be treated as an extra independent pre-extraction data flip that would always be diagnosed normally.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
