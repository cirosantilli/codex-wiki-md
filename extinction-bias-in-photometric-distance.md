# Extinction bias in photometric distance

↑ **Parent:** [Distance modulus](distance-modulus.md)

Let $A\geq0$ be the [interstellar extinction](interstellar-extinction.md) in magnitudes in the specified [photometric passband](photometric-passband.md). Compared with the same unobscured source at the same distance, its [radiative flux](radiative-flux.md) is multiplied by $10^{-0.4A}$, so its [apparent magnitude](apparent-magnitude.md) increases by $A$. Consequently,

$$
m-M=5\log_{10}\left(\frac{d}{10\,\mathrm{pc}}\right)+A,\qquad \mu_0=m-M-A.
$$

Here $\mu_0$ is the extinction-corrected [distance modulus](distance-modulus.md). The correction subtracts $A$ before using the distance formula. Caltech's NED distance-method documentation explicitly distinguishes an apparent [distance modulus](distance-modulus.md) from an extinction-corrected [distance modulus](distance-modulus.md). [NASA/IPAC NED: Cepheid apparent and reddening-corrected distances](https://ned.ipac.caltech.edu/Library/Distances/distintro.html).

Ignoring positive [interstellar extinction](interstellar-extinction.md) attributes too much dimming to distance, producing an overestimate:

$$
\frac{d_{\mathrm{inferred}}}{d}=10^{A/5}.
$$

As an illustrative toy, put the source with $M=0$ at $100$ [parsecs](parsec.md) behind $A=1$ magnitude of [interstellar extinction](interstellar-extinction.md). The measured [apparent magnitude](apparent-magnitude.md) is $m=6$. Setting $A=0$ incorrectly gives $d_{\mathrm{inferred}}=10\,\mathrm{pc}\times10^{6/5}\simeq158.489\,\mathrm{pc}$, a factor $1.584893$ too large. Subtracting the known $A=1$ recovers $100$ [parsecs](parsec.md). The diagram's fixed $A=1$ offset is a controlled illustration, not a model of how actual [interstellar extinction](interstellar-extinction.md) grows with distance, and none of its values are [star](star.md) catalogue measurements.

## ↑ Ancestors (6)

1. [Distance modulus](distance-modulus.md)
2. [Astronomical magnitude](astronomical-magnitude.md)
3. [Astrophysics](astrophysics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Distance modulus](distance-modulus.md)
