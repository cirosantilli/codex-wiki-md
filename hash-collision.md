# Hash collision

↑ **Parent:** [Hash function](hash-function.md)

A hash collision is a [function collision](function-collision.md) of a [hash function](hash-function.md) $h:U\to B$: two distinct [inputs](input-computer-science.md) $x,y\in U$ have the same [output](output-computing.md), $h(x)=h(y)$. Repeating the same [input](input-computer-science.md) is not a [hash collision](hash-collision.md). Unequal hash values prove the keys differ; equal hash values only identify candidates that might be equal. This makes a [hash function](hash-function.md) useful as a compact filter before comparing the original data.

Here is a deliberately simple example using [modular arithmetic](modular-arithmetic-split.md). Let $h(k)=k\bmod16$ for nonnegative [integer](integer-split.md) keys, and let a four-bucket [hash table](hash-table.md) use the further bucket index $b(k)=h(k)\bmod4$. For keys $2,6,18$, the hash values are $2,6,2$, while all three bucket indices are $2$. Thus $2$ and $18$ form a [hash collision](hash-collision.md) for $h$; $2$ and $6$ share a table bucket even though their full hash values differ. Always specify which [function](function-split.md) is being compared: a table collision concerns the bucket-index [function](function-split.md), which may discard more information than the original [hash function](hash-function.md).

<a id="image-a-shared-hash-value-and-a-shared-table-bucket-discard-different-distinctions"></a>
![](hash-collision-key-identity.png)

**[Figure 18](#image-a-shared-hash-value-and-a-shared-table-bucket-discard-different-distinctions). A shared hash value and a shared table bucket discard different distinctions**. Constructed [integer](integer-split.md) keys $2,6,18$ pass through $h(k)=k\bmod16$ and $b(k)=h(k)\bmod4$. Orange highlights the [hash collision](hash-collision.md) between $2$ and $18$; blue key $6$ joins them only after bucket reduction. [Separate chaining](separate-chaining.md) retains all three keys. This is a toy calculation, not a measured workload or a [cryptographic hash function](cryptographic-hash-function.md).

With [separate chaining](separate-chaining.md), bucket $2$ holds all three records in a [linked list](linked-list.md). A search for $18$ visits that bucket and compares the stored keys until it finds $18$; a search for $34$ visits the same bucket but rejects every stored key. A [hash collision](hash-collision.md) changes the search work, while key comparison preserves correctness. Storing only one record per hash value would incorrectly merge distinct keys. This is the purpose of collision handling in a [hash table](hash-table.md).[Lecture 8: Hashing I](6-006-introduction-to-algorithms-fall-2011-by-massachusetts-institute-of-technology-6-006-course-staff/lecture-8-hashing-i.md)

The [pigeonhole principle](pigeonhole-principle.md) explains inevitability: if a [hash function](hash-function.md) has only $M$ possible [outputs](output-computing.md), any $M+1$ distinct [inputs](input-computer-science.md) contain a [hash collision](hash-collision.md). In particular, a [function](function-split.md) whose [domain of a function](domain-of-a-function.md) is larger than its finite [codomain](codomain.md) cannot be an [injective function](injective-function.md). This is an existence statement; it gives neither an efficient way to find the pair nor a [probability](probability.md) for a smaller collection of keys. A particular small collection might have no [hash collision](hash-collision.md) at all.

For a [cryptographic hash function](cryptographic-hash-function.md), [collision resistance](collision-resistance.md) asks that finding any two distinct messages with equal full digests be computationally infeasible under the specified model and resources. It does not mean that [hash collisions](hash-collision.md) do not exist. [Preimage resistance](preimage-resistance.md) asks a different question: given a target digest $t$, how hard is it to find a message $x$ with $h(x)=t$? The collision finder may choose both messages and their common digest; the [preimage](preimage.md) finder is given the digest in advance. These definitions distinguish two search tasks, independently of how a [hash table](hash-table.md) stores records.[Quynh Dang, NIST SP 800-107 Revision 1 (2012), section 3.1 and section 4.1, definitions of collision and preimage resistance](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-107r1.pdf)

**Table of contents**

- [Birthday probability for hash outputs](birthday-probability-for-hash-outputs.md)

## ↑ Ancestors (3)

1. [Hash function](hash-function.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Birthday probability for hash outputs](birthday-probability-for-hash-outputs.md)
- [Birthday problem](birthday-problem.md)
- [Hash collision](hash-collision.md)
- [Hash function](hash-function.md)
- [Hash table](hash-table.md)
- [Key equality](key-equality.md)
- [Linear probing](linear-probing.md)
- [Linear probing cluster](linear-probing-cluster.md)
- [Memoization arithmetic and stack costs](memoization-arithmetic-and-stack-costs.md)
- [Memoization key](memoization-key.md)
- [Primary clustering](primary-clustering.md)
- [Separate chaining](separate-chaining.md)
- [Tombstone in open addressing](tombstone-in-open-addressing.md)
