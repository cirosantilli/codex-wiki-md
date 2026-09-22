# Add with carry

↑ **Parent:** [Carry flag](carry-flag.md)

For $n$-bit operands, an [add with carry](add-with-carry.md) operation forms $X+Y+C_{\rm in}$, retains its residue [modulo](modulo-operation.md) $2^n$, and outputs its [arithmetic carry](carry-arithmetic.md). Adding low limbs first and feeding each [arithmetic carry](carry-arithmetic.md) into the next limb implements multiword unsigned addition. With $M=2^n$, the identities $X_0+Y_0=Z_0+Mc$ and $X_1+Y_1+c=Z_1+Md$ combine into $(MX_1+X_0)+(MY_1+Y_0)=MZ_1+Z_0+M^2d$.[Page 1, Add with carry](thumb-16-bit-instruction-set-quick-reference-by-arm.md)

## ↑ Ancestors (5)

1. [Carry flag](carry-flag.md)
2. [Processor register](processor-register.md)
3. [Central processing unit](central-processing-unit.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Add with carry](add-with-carry.md)
