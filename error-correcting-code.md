# Error-correcting code

↑ **Parent:** [Binary block code](binary-block-code.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Error-correcting_code)

An error-correcting code is a set of [codewords](codeword.md) chosen with enough separation to recover a transmitted message after specified errors. For equal-length words and bit-flip errors, separation is measured by [Hamming distance](hamming-distance.md). If the [minimum distance](minimum-distance-of-a-code.md) is $d$, any nonzero pattern of at most $d-1$ flips changes a valid word into an invalid word and can therefore be detected. Every pattern of at most $t=\lfloor(d-1)/2\rfloor$ flips can be corrected by choosing the unique nearby [codeword](codeword.md).

The distinction matters. A distance-two code detects a single flip but need not locate it; a distance-three code corrects a single flip. The [triangle inequality](triangle-inequality.md) explains the correction threshold: a received word within distance $t$ of two distinct [codewords](codeword.md) would put those [codewords](codeword.md) within distance $2t<d$, a contradiction. Actual decoders also need an efficient way to find the nearby word; a [parity-check matrix](parity-check-matrix.md) and [syndrome decoding](syndrome-decoding.md) exploit the structure of a [linear code](linear-code.md) to do this.

**Table of contents**

- [Repetition code](repetition-code.md)

## ↑ Ancestors (7)

1. [Binary block code](binary-block-code.md)
2. [Block code](block-code.md)
3. [Coding theory](coding-theory-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Channel coding](channel-coding.md)
- [Finite field](finite-field.md)
- [Hamming cube as an L1 and L2 metric](hamming-cube-as-an-l1-and-l2-metric.md)
- [Number theory](number-theory-split.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-35/2/solution.md)
- [Repetition code](repetition-code.md)
