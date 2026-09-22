# Key equality

↑ **Parent:** [Hash table](hash-table.md)

The [equivalence relation](equivalence-relation.md) used to decide whether two keys name the same record. A [hash function](hash-function.md) must respect [key equality](key-equality.md); a [hash collision](hash-collision.md) does not establish [key equality](key-equality.md).

The choice of [key equality](key-equality.md) is part of the map's meaning. In the one-value-per-key policy of [hash table](hash-table.md), one record represents each stored [equivalence class](equivalence-class.md) of keys: `put(k,v)` updates an existing equal key and adds a record only if no equal key is present. A collection that deliberately retains repeated equal keys has a different policy; its load count must count those extra records too. Repeated calls and distinct stored records are different quantities.[6.006 Introduction to Algorithms, Fall 2011 by Massachusetts Institute of Technology, 6.006 course staff; p. 1, Dictionary Problem: distinct keys or replacement on repeated insertion](6-006-introduction-to-algorithms-fall-2011-by-massachusetts-institute-of-technology-6-006-course-staff/lecture-8-hashing-i.md)

For an original example, restrict keys to two-letter [strings](string.md) using letters `A` through `Z` or `a` through `z`. Declare two keys equal when replacing every uppercase letter by its lowercase counterpart gives the same [string](string.md). Assign each letter its position $1,\ldots,26$ in the alphabet, ignoring case, and define the bucket-index [hash function](hash-function.md) as the sum of the two positions modulo $8$, using [modular arithmetic](modular-arithmetic-split.md). Then `AB` and `ab` are equal keys and both select [hash bucket](hash-bucket.md) $3$. Key `ba` also selects [hash bucket](hash-bucket.md) $3$ because $2+1=3$, but is unequal to `ab`: order still matters. Starting empty, `put(AB,7)`, `put(ab,9)`, `put(ba,4)` leave two records, with values $9$ for the `ab` [equivalence class](equivalence-class.md) and $4$ for `ba`; the [hash table load factor](load-factor-of-a-hash-table.md) is $2/8=1/4$, not $3/8$.

The compatibility rule is one-way: $x\sim y\Rightarrow h_m(x)=h_m(y)$. Otherwise a lookup using an equal spelling could search a different [hash bucket](hash-bucket.md) and incorrectly report absence. Equal indices merely allow a [key equality](key-equality.md) check. Both the [equivalence relation](equivalence-relation.md) and the [hash function](hash-function.md) must stay consistent while records are stored; changing equality-relevant key contents can invalidate the lookup rule. The Java contract imposes these consistency and equality requirements on `equals` and `hashCode`.[Java Platform, Standard Edition 25 API Specification by Oracle; Method Details, equals equivalence-relation contract and hashCode general contract](java-platform-standard-edition-25-api-specification-by-oracle/object-java-se-25-and-jdk-25.md)

## ↑ Ancestors (4)

1. [Hash table](hash-table.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Hash table](hash-table.md)
- [Hash table key](hash-table-key.md)
- [Hash table record](hash-table-record.md)
- [Key equality](key-equality.md)
- [Linear probing](linear-probing.md)
- [Linear probing cluster](linear-probing-cluster.md)
- [Load factor of a hash table](load-factor-of-a-hash-table.md)
- [Memoization key](memoization-key.md)
- [Separate chaining](separate-chaining.md)
- [Tombstone in open addressing](tombstone-in-open-addressing.md)
