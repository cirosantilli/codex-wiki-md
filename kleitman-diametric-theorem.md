# Kleitman diametric theorem

↑ **Parent:** [Boolean lattice](boolean-lattice.md)

A family in the Boolean lattice whose pairwise Hamming distances are at most $d<n$ has size at most $D(n,d)$. Downward compression followed by [elementary set shifts](elementary-set-shift.md) preserves the distance bound. In the resulting down-set, the section containing the last coordinate has diameter at most $d-2$: two members leave a coordinate free, and shifting the last coordinate to it creates a pair with two additional disagreements. This gives the recurrence $D(n,d)=D(n-1,d)+D(n-1,d-2)$. The boundary case $d=n-1$ follows by pairing complementary sets. Hamming balls attain the even case; the union of two radius-$q$ balls with adjacent centers attains the odd case.

## ↑ Ancestors (7)

1. [Boolean lattice](boolean-lattice.md)
2. [Set family](set-family.md)
3. [Extremal set theory](extremal-set-theory-split.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Nonuniform t-intersecting family bound](nonuniform-t-intersecting-family-bound.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-14/2/solution.md)
