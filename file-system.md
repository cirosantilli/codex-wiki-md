# File system

↑ **Parent:** [Operating system](operating-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/File_system)

A [file system](file-system.md) organizes [files](#computer-file), their [file metadata](#file-metadata), and the names through which they can be found. In the [Unix](operating-system.md#unix) model used here, a [file-system directory](#file-system-directory) contains [directory entries](#directory-entry) associating names with [inodes](#inode); an [inode](#inode) describes the underlying [file](#computer-file) and how to locate its contents. The [file-system namespace](#file-system-namespace) answers "what does this name reach?", while the [inode](#inode) answers "which [file](#computer-file) is it?". These are distinct responsibilities, even though they cooperate on every lookup.

For a computed toy example, let one [file-system directory](#file-system-directory) contain names `a` and `b`, both referring to [inode](#inode) 42 in the same [file system](file-system.md). That [inode](#inode) has size 6 [bytes](computer-science.md#byte) and two [hard links](#hard-link). Its direct references lead to four-[byte](computer-science.md#byte) [file data blocks](#file-data-block) 7 and 9: block 7 holds `hell`, while block 9 holds `o` followed by a newline, with two unused slots. Reading either name therefore obtains the same six-[byte](computer-science.md#byte) contents `hello` followed by a newline. There is one [file](#computer-file) with two names, not two copies. This direct-reference layout and tiny block size are teaching choices, not requirements on every [file system](file-system.md).

<a id="image-two-hard-links-reach-one-inode-a-file-descriptor-reaches-it-through-an-open-file-description"></a>
![](file-system-inodes-and-hard-links.png)

**[Figure 1](#image-two-hard-links-reach-one-inode-a-file-descriptor-reaches-it-through-an-open-file-description). Two hard links reach one inode; a file descriptor reaches it through an open file description**.

The separation is useful because a rename within this [file system](file-system.md), from `a` to a previously unused name `c`, can change a [directory entry](#directory-entry) without copying the six [bytes](computer-science.md#byte) of contents. The remaining name `b` still reaches [inode](#inode) 42. A successful write changing the first [byte](computer-science.md#byte) through either name changes what both names subsequently read, to `jello` followed by a newline. This sharing is the attraction of [hard links](#hard-link), and also why a [hard link](#hard-link) is not an independent backup. A program that replaces a named [file](#computer-file) with a different [file](#computer-file) can instead make the names diverge. [The Open Group, POSIX.1-2024, rename: changing names and replacing directory entries](https://pubs.opengroup.org/onlinepubs/9799919799/functions/rename.html)

**Table of contents**

- [Computer file](#computer-file)
  - [File offset](#file-offset)
  - [File metadata](#file-metadata)
  - [File data block](#file-data-block)
- [File-system directory](#file-system-directory)
  - [Directory entry](#directory-entry)
- [File-system namespace](#file-system-namespace)
  - [Hard link](#hard-link)
    - [Unlinking an open file](#unlinking-an-open-file)
  - [Symbolic link](#symbolic-link)
- [Buffer cache](#buffer-cache)
  - [Buffered device block](#buffered-device-block)
    - [Buffer cache key](#buffer-cache-key)
    - [Buffer cache validity](#buffer-cache-validity)
    - [Dirty buffer](#dirty-buffer)
    - [Clean buffer](#clean-buffer)
    - [Pinned buffer](#pinned-buffer)
  - [Buffer cache writeback](#buffer-cache-writeback)
  - [Buffer cache eviction](#buffer-cache-eviction)
  - [Buffer cache state model](#buffer-cache-state-model)
    - [Buffer cache access trace](#buffer-cache-access-trace)
  - [xv6 buffer cache](#xv6-buffer-cache)
  - [Page cache](#page-cache)
    - [Linux buffer head](#linux-buffer-head)
    - [Linux folio](#linux-folio)
    - [iomap](#iomap)
- [File-system journaling](#file-system-journaling)
  - [File-system crash consistency](#file-system-crash-consistency)
  - [File-system transaction](#file-system-transaction)
    - [File-system transaction durability](#file-system-transaction-durability)
      - [fsync](#fsync)
  - [Write-ahead logging](#write-ahead-logging)
    - [Journal payload](#journal-payload)
    - [Journal commit record](#journal-commit-record)
    - [Journal checkpoint](#journal-checkpoint)
    - [Journal replay](#journal-replay)
  - [File-system journaling mode](#file-system-journaling-mode)
- [File-system allocation bitmap](#file-system-allocation-bitmap)
  - [Block allocation bitmap](#block-allocation-bitmap)
  - [Inode allocation bitmap](#inode-allocation-bitmap)
- [Storage flush](#storage-flush)
- [Atomic storage write](#atomic-storage-write)
- [ext4](#ext4)
- [File-system backup](#file-system-backup)
- [Access control list](#access-control-list)
- [File Allocation Table](#file-allocation-table)
  - [FAT32](#fat32)
- [NTFS](#ntfs)
- [Inode](#inode)

## Computer file

↑ **Parent:** [File system](file-system.md)

An object whose contents and attributes can be accessed through [operating system](operating-system.md) interfaces. Here an ordinary [file](#computer-file) means a [byte](computer-science.md#byte) sequence with [file metadata](#file-metadata), distinct from a [file-system directory](#file-system-directory) or a [symbolic link](#symbolic-link). Its contents need not disappear when the creating [operating-system process](operating-system.md#process-computing) ends.

### File offset

↑ **Parent:** [Computer file](#computer-file)

A [byte](computer-science.md#byte) position measured from the start of a [file](#computer-file), beginning at zero. A [memory-mapped file](virtual-memory.md#memory-mapped-file) combines a starting [file offset](#file-offset) with a displacement inside its mapping; this is distinct from an [open file description](operating-system.md#open-file-description)'s current read/write position.

### File metadata

↑ **Parent:** [Computer file](#computer-file)

Information describing a [file](#computer-file), such as type, owner, access permissions, size, timestamps and [hard link](#hard-link) count. In the toy layout, the [inode](#inode) carries these attributes; the [directory entries](#directory-entry) carry the names. The distinction matters because renaming a [file](#computer-file) need not copy its contents.

### File data block

↑ **Parent:** [Computer file](#computer-file)

A storage unit holding part of a [file](#computer-file)'s contents. The toy [inode](#inode) references two four-[byte](computer-science.md#byte) [file data blocks](#file-data-block) for six [bytes](computer-science.md#byte) of contents: allocated capacity is $2\cdot4=8$ [bytes](computer-science.md#byte), while logical size is $4+2=6$ [bytes](computer-science.md#byte). This counts only the two [file data blocks](#file-data-block), excluding storage for the [inode](#inode) and [directory entries](#directory-entry).

## File-system directory

↑ **Parent:** [File system](file-system.md)

A [file](#computer-file) containing [directory entries](#directory-entry). Each entry supplies a name in that [file-system directory](#file-system-directory); two entries in the same [file-system directory](#file-system-directory) cannot have the same name. In an [inode](#inode)-based [file system](file-system.md), a [file-system directory](#file-system-directory) has its own [inode](#inode), and its contents describe names of other objects. [The Open Group, POSIX.1-2024, sections 3.103–3.104: directory and directory entry](https://pubs.opengroup.org/onlinepubs/9799919799/basedefs/V1_chap03.html#tag_03_103)

### Directory entry

↑ **Parent:** [File-system directory](#file-system-directory)

An association between a name in a [file-system directory](#file-system-directory) and a [file](#computer-file). In the toy [file system](file-system.md), the pairs are `(a, 42)` and `(b, 42)`: each name resolves to the same [inode](#inode). The name belongs to the [directory entry](#directory-entry), rather than being the single authoritative name stored in that [inode](#inode).

## File-system namespace

↑ **Parent:** [File system](file-system.md)

The organization of names and the rules for resolving them to [files](#computer-file). A path such as `/notes/a` selects successive [directory entries](#directory-entry) starting from the root [file-system directory](#file-system-directory). Its spelling describes a route, not an immutable identity: replacing the final [directory entry](#directory-entry) can make the same path reach a different [inode](#inode).

### Hard link

↑ **Parent:** [File-system namespace](#file-system-namespace)

A [directory entry](#directory-entry) associating a name directly with an existing [file](#computer-file). In the [inode](#inode)-based example, successful `link("a", "b")` adds the second name for [inode](#inode) 42 and increases its [hard link](#hard-link) count from 1 to 2. Both [directory entries](#directory-entry) have equal status; removing `a` leaves `b` usable. This example assumes both names are in the same [file system](file-system.md), the destination name is unused, and the operation is permitted. [The Open Group, POSIX.1-2017, link: adding a directory entry and incrementing the link count](https://pubs.opengroup.org/onlinepubs/9699919799/functions/link.html)

#### Unlinking an open file

↑ **Parent:** [Hard link](#hard-link)

For an ordinary [file](#computer-file) under the [POSIX](operating-system.md#posix) rules used here, successful `unlink("a")` removes the named [directory entry](#directory-entry) and decreases the [hard link](#hard-link) count. An existing [open file description](operating-system.md#open-file-description) still refers to the same [file](#computer-file); removing a name does not detach an already open [file descriptor](operating-system.md#file-descriptor). When the final [hard link](#hard-link) disappears, the contents remain available through open references until those references close. This distinction is between the lifetime of a name and the lifetime of the underlying [file](#computer-file). [The Open Group, POSIX.1-2017, unlink: removal of names and deferred removal of open-file contents](https://pubs.opengroup.org/onlinepubs/9699919799/functions/unlink.html)

Start with names `a` and `b` for [inode](#inode) 42 and one [file descriptor](operating-system.md#file-descriptor) `3` referring to one [open file description](operating-system.md#open-file-description). Let $L$ count [hard links](#hard-link) and $O$ count live [open file descriptions](operating-system.md#open-file-description) for this [file](#computer-file). Assume successful operations, no additional references, and no [memory-mapped file](virtual-memory.md#memory-mapped-file). The stages are

$$
(L,O):\quad (2,1)\xrightarrow{\mathrm{unlink}(a)}(1,1)\xrightarrow{\mathrm{unlink}(b)}(0,1)\xrightarrow{\mathrm{close}(3)}(0,0).
$$

After the first removal, `b` still works. After the second, neither name works, but a read through the existing [file descriptor](operating-system.md#file-descriptor) can still obtain all six [bytes](computer-science.md#byte) if its [open file description](operating-system.md#open-file-description)'s current position is at the beginning. The final close releases the last open reference, allowing the [inode](#inode) and its [file data blocks](#file-data-block) to be reclaimed. Freed storage is reusable; this does not promise that old [bytes](computer-science.md#byte) are securely erased. [The Open Group, POSIX, close: releasing descriptors, open file descriptions and unlinked-file storage](https://pubs.opengroup.org/onlinepubs/009604499/functions/close.html)

<a id="image-hard-link-and-open-reference-counts-distinguish-removal-of-names-from-reclamation-of-a-file"></a>
![](unlink-open-file-lifetime.png)

**[Figure 2](#image-hard-link-and-open-reference-counts-distinguish-removal-of-names-from-reclamation-of-a-file). Hard link and open-reference counts distinguish removal of names from reclamation of a file**.

The reasoning is bookkeeping rather than a long proof: each successful removal subtracts one from $L$ and leaves $O$ unchanged; closing the only [file descriptor](operating-system.md#file-descriptor) in this example releases the sole [open file description](operating-system.md#open-file-description). Storage is reclaimable only at the last stage. $O$ is a teaching count, not a count of [file descriptors](operating-system.md#file-descriptor) or an asserted internal [inode](#inode) field: several [file descriptors](operating-system.md#file-descriptor) can share one [open file description](operating-system.md#open-file-description), and other references such as a [memory-mapped file](virtual-memory.md#memory-mapped-file) require additional lifetime accounting. The diagrams are abstract models, not operations on actual user [files](#computer-file).

### Symbolic link

↑ **Parent:** [File-system namespace](#file-system-namespace)

A separate [file](#computer-file) containing a path string to be interpreted during lookup. A [symbolic link](#symbolic-link) to `a` stores that spelling rather than adding another [hard link](#hard-link) to [inode](#inode) 42; it can remain after `a` disappears and then fail to reach a target. It does not increase the target's [hard link](#hard-link) count. The diagrams below track only [hard links](#hard-link) and open references. [The Open Group, POSIX, symlink: storing the supplied path string](https://pubs.opengroup.org/onlinepubs/009695299/functions/symlink.html)

// Target: computer-science.bigb

## Buffer cache

↑ **Parent:** [File system](file-system.md)

A memory cache of device blocks indexed by device identity and block number. A hit avoids slow device access; a miss obtains a buffer and reads the block. Dirty buffers carry modified data that must be written before reuse, and pinned buffers cannot be evicted while an operation uses them. Deferred writes improve throughput but need explicit durability handling.

A [buffer cache](#buffer-cache) can hold both [file data blocks](#file-data-block) and storage containing [file metadata](#file-metadata), such as [inodes](#inode) and [block allocation bitmaps](#block-allocation-bitmap). Reusing a [buffered device block](#buffered-device-block) saves repeated [input-output](computer-science.md#input-output); retaining several modifications before [buffer cache writeback](#buffer-cache-writeback) can combine them into one transfer. Section 40.7 of [Operating Systems: Three Easy Pieces by Remzi H. Arpaci-Dusseau and others](computer-science-bibliography.md#operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others) explains these benefits for [file systems](file-system.md).[pp. 14–16: caching and buffering](computer-science-bibliography.md#operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/file-system-implementation)

The central distinction is that a [dirty buffer](#dirty-buffer) needs a write, whereas a [pinned buffer](#pinned-buffer) must retain its identity. A [clean buffer](#clean-buffer) can still be pinned, and a [dirty buffer](#dirty-buffer) can have no client references. Neither releasing a reference nor obtaining a [cache hit](computer-science.md#cache-hit) establishes [file-system transaction durability](#file-system-transaction-durability).

### Buffered device block

↑ **Parent:** [Buffer cache](#buffer-cache)

A [data structure](data-structure.md) holding the contents of one fixed-size region of a storage device, together with its [buffer cache key](#buffer-cache-key), [buffer cache validity](#buffer-cache-validity), modification state and lifetime information. A storage region containing [file metadata](#file-metadata) is just as eligible as a [file data block](#file-data-block). The structure can survive many callers: releasing it usually makes it available for later reuse, rather than immediately deleting the cached contents.

#### Buffer cache key

↑ **Parent:** [Buffered device block](#buffered-device-block)

The identity used to find a [buffered device block](#buffered-device-block). In the fixed-block-size model, $d$ identifies the device and $b$ its block number; $(d_1,7)$ and $(d_2,7)$ are different keys if $d_1\ne d_2$. A [file](#computer-file)'s pathname or its logical block offset alone is insufficient for this device-indexed model. Interfaces supporting different transfer sizes need to specify the size and overlap rules too.

Maintain at most one logical [buffered device block](#buffered-device-block) for each [buffer cache key](#buffer-cache-key) within this [buffer cache](#buffer-cache). Otherwise two callers could modify different copies and later overwrite one another's changes. Lookup and reservation must therefore be coordinated by [synchronization](operating-system.md#synchronization-computing): even before contents are ready, a reserved key directs a second caller to the same structure. This invariant concerns the participating cache, not every copy of those [bytes](computer-science.md#byte) anywhere in the machine.

#### Buffer cache validity

↑ **Parent:** [Buffered device block](#buffered-device-block)

Whether a [buffered device block](#buffered-device-block)'s contents are ready for the requested use. Reserving a [buffer cache key](#buffer-cache-key) does not make its previous occupant's contents valid. A read fills the reserved structure before exposing its contents. A second caller finding an unfinished fill must wait; finding the identity is not yet a data [cache hit](computer-science.md#cache-hit) under the convention used here. A failed fill must not expose the stale contents as valid.

A buffered partial write first needs the untouched [bytes](computer-science.md#byte): read the old contents on a [cache miss](computer-science.md#cache-miss), change the requested range, and retain the result as a [dirty buffer](#dirty-buffer). A complete overwrite can initialize every [byte](computer-science.md#byte) without reading the old contents if the interface permits that path. The [buffer cache access trace](#buffer-cache-access-trace) deliberately uses partial writes, so every [cache miss](computer-science.md#cache-miss) reads the old block.

#### Dirty buffer

↑ **Parent:** [Buffered device block](#buffered-device-block)

A valid [buffered device block](#buffered-device-block) with modifications still owed to its backing location. Until successful [buffer cache writeback](#buffer-cache-writeback), simply reassigning its [buffer cache key](#buffer-cache-key) would lose those modifications. “Dirty” records a write obligation; a write of identical contents can still mark the structure dirty. Repeated buffered writes can leave only the latest contents to be transferred.

#### Clean buffer

↑ **Parent:** [Buffered device block](#buffered-device-block)

A valid [buffered device block](#buffered-device-block) with no outstanding write obligation to the backing location tracked by this cache. It can serve a [cache hit](computer-science.md#cache-hit). It becomes eligible for [buffer cache eviction](#buffer-cache-eviction) only when its retention and any pending [input-output](computer-science.md#input-output) permit reuse. “Clean” does not assert that a device's volatile [memory cache](computer-science.md#cache-computing) has been flushed to persistent storage.

#### Pinned buffer

↑ **Parent:** [Buffered device block](#buffered-device-block)

A [buffered device block](#buffered-device-block) whose identity is retained for unfinished work. [Reference counting](computer-science.md#reference-counting) can represent both client references and additional pins. Dropping a client reference does not release an outstanding journal pin; dropping a pin does not remove somebody else's reference. In the [buffer cache state model](#buffer-cache-state-model), $r$ counts all such retained references, so $r>0$ prevents [buffer cache eviction](#buffer-cache-eviction). This count keeps the structure alive; a [mutex](operating-system.md#mutex) separately controls who can inspect or change its contents. Waiting callers also need lifetime protection.

### Buffer cache writeback

↑ **Parent:** [Buffer cache](#buffer-cache)

Transferring a [dirty buffer](#dirty-buffer)'s current contents to its backing location. The [buffer cache state model](#buffer-cache-state-model) permits no concurrent modification during the transfer and marks the result clean only after successful completion. A failed write preserves the obligation and prevents the proposed [buffer cache eviction](#buffer-cache-eviction). A production implementation allowing new writes during [input-output](computer-science.md#input-output) must retain their obligation rather than incorrectly clearing it when an older transfer finishes.

A successful transfer can leave data in a device's volatile [memory cache](computer-science.md#cache-computing). A [storage flush](#storage-flush) or the documented equivalent supplies a persistence boundary; [file-system journaling](#file-system-journaling) supplies recovery rules for related updates. These are additional obligations, not consequences of becoming a [clean buffer](#clean-buffer).[Explicit volatile write back cache control by The kernel development community](computer-science-bibliography.md#explicit-volatile-write-back-cache-control-by-the-kernel-development-community)

### Buffer cache eviction

↑ **Parent:** [Buffer cache](#buffer-cache)

Removing a [buffer cache key](#buffer-cache-key)'s resident contents so the storage in [computer memory](computer-science.md#computer-memory) can serve another key. An unreferenced [clean buffer](#clean-buffer) can be reused directly in the [buffer cache state model](#buffer-cache-state-model); an unreferenced [dirty buffer](#dirty-buffer) requires successful [buffer cache writeback](#buffer-cache-writeback) first. A [pinned buffer](#pinned-buffer) cannot be chosen regardless of cleanliness. [LRU replacement](virtual-memory.md#lru-replacement) ranks eligible candidates; it does not override lifetime protection. If every candidate is retained, a [cache miss](computer-science.md#cache-miss) cannot obtain space until something releases a reference or capacity changes. This is a resource shortage, not permission to discard live contents.

### Buffer cache state model

↑ **Parent:** [Buffer cache](#buffer-cache)

Use one fixed-size [buffered device block](#buffered-device-block) per [buffer cache key](#buffer-cache-key), serialized operations, successful reads and writes, and no outside changes to the backing contents. Record an absent state or a reserved key with validity $v$, dirty flag $D$, and retained-reference count $r$. The [bits](information-theory.md#bit) $v,D$ describe contents, while the nonnegative [integer](integer.md) $r$ describes lifetime. Every [dirty buffer](#dirty-buffer) is valid, so $D=1$ implies $v=1$. Reservation begins at $(v,D,r)=(0,0,1)$; successful fill changes only $v$ to 1. Modifying a valid retained structure sets $D=1$. Releasing a caller changes $r$, not $v$ or $D$.

<a id="image-buffer-cache-validity-dirty-buffers-and-retained-references-impose-different-state-transition-rules"></a>
![](buffer-cache-block-state-transitions.png)

**[Figure 3](#image-buffer-cache-validity-dirty-buffers-and-retained-references-impose-different-state-transition-rules). Buffer cache validity, dirty buffers and retained references impose different state-transition rules**.

The first diagram separates contents transitions from reference transitions. [Buffer cache writeback](#buffer-cache-writeback) temporarily retains the structure while transferring its contents; that internal reference is acquired and released inside the single serialized operation shown. [Buffer cache eviction](#buffer-cache-eviction) requires a valid [clean buffer](#clean-buffer) with $r=0$. The diagram omits read errors, explicit cancellation of invalid reservations, concurrent writes, invalidation and journal ordering. In particular, a journal can forbid otherwise possible [buffer cache writeback](#buffer-cache-writeback) until its [write-ahead logging](#write-ahead-logging) dependencies are satisfied.

For a small independent check, bound $r$ to $0,1,2$. Starting absent, allow reservation, acquisition, successful fill, modification, successful [buffer cache writeback](#buffer-cache-writeback), release of a valid retained structure, and eligible [buffer cache eviction](#buffer-cache-eviction). Exactly nine abstract states are reachable: absent, two invalid reservations with $r=1,2$, and six valid states combining $D=0,1$ with $r=0,1,2$. Every transition preserves $D\le v$; the only eviction source has $(v,D,r)=(1,0,0)$. This bounded [finite-state machine](foundations-of-mathematics.md#finite-state-machine) check supports these safety rules, not a claim that work always completes.

#### Buffer cache access trace

↑ **Parent:** [Buffer cache state model](#buffer-cache-state-model)

Let $A,B,C$ be three distinct [buffer cache keys](#buffer-cache-key) on one device. Use two initially empty slots, [LRU replacement](virtual-memory.md#lru-replacement) refreshed at each completed request, and synchronous successful [buffer cache writeback](#buffer-cache-writeback) of a dirty victim. Each request acquires its target, finishes any fill, reads or partially modifies it, and releases the client reference. An explicit pin on $A$ remains after request 2 through request 7; pin and unpin do not refresh recency. No other references, invalidations, background writes or durability operations occur. Initial backing contents are represented by the [integers](integer.md) $A=10,B=20,C=30$; partial writes change the tracked value of $A$ to 11 and then 12 while preserving the unshown remainder.

<a id="image-exact-cache-hits-cache-misses-retained-references-and-buffer-cache-evictions-in-a-two-slot-buffer-cache"></a>
![](buffer-cache-pinned-dirty-eviction-trace.png)

**[Figure 4](#image-exact-cache-hits-cache-misses-retained-references-and-buffer-cache-evictions-in-a-two-slot-buffer-cache). Exact cache hits, cache misses, retained references and buffer cache evictions in a two-slot buffer cache**.

The eight data requests are read $A$, write $A=11$, read $B$, read $C$, read $A$, write $A=12$, read $C$, and read $B$ after unpinning $A$. They yield four [cache hits](computer-science.md#cache-hit), four [cache misses](computer-science.md#cache-miss), four device reads and one device write. The pin and unpin are lifetime operations, excluded from the data-request count. At the read of $C$, $A$ is older than $B$ but pinned, so the [clean buffer](#clean-buffer) for $B$ is evicted instead. Reading $A$ then returns 11 without device access even though its backing value is still 10. The second write supersedes 11; reading $C$ makes $A$ the older entry again. After unpinning, the final read of $B$ writes back 12 before evicting $A$. After that request, backing $A$ contains 12, while the resident keys are $C,B$.

This example exposes the value of retaining modified contents: a [cache hit](computer-science.md#cache-hit) can return a newer value than a device read would. It also exposes the cost of [reference counting](computer-science.md#reference-counting) constraints: a pinned older entry forces a different victim. An independent capacity sweep gives two [cache hits](computer-science.md#cache-hit), six [cache misses](computer-science.md#cache-miss) and two device writes with one slot and no pin, but three [cache hits](computer-science.md#cache-hit), five [cache misses](computer-science.md#cache-miss) and two device writes with two slots and no pin. With one slot and the stipulated pin, the read of $B$ cannot proceed. With three slots, both pin choices give five [cache hits](computer-science.md#cache-hit), three [cache misses](computer-science.md#cache-miss) and no eviction-triggered write; $A$ remains dirty with value 12, so the absence of a device write does not establish [file-system transaction durability](#file-system-transaction-durability).

### xv6 buffer cache

↑ **Parent:** [Buffer cache](#buffer-cache)

The teaching implementation's `bget` checks device and block number under a shared [spinlock](operating-system.md#spinlock), increments `refcnt` before releasing that lock, and then takes the buffer's content [mutex](operating-system.md#mutex). On a [cache miss](computer-science.md#cache-miss) it reserves an unused structure and clears `valid`; `bread` fills it only if necessary. This makes lookup and reservation share one [synchronization](operating-system.md#synchronization-computing) boundary. `brelse` releases the content [mutex](operating-system.md#mutex) and decrements the reference count. Unlike the stipulated trace policy, it moves the structure to the recent end only when that decrement reaches zero. [bio.c](computer-science-bibliography.md#xv6-risc-v-source-code/bio-c)

This implementation has `valid` and `refcnt` but no generic dirty flag. Its [file-system journaling](#file-system-journaling) code records modified blocks with `log_write`, pins each newly recorded block, copies cached contents to the journal during commit, and unpins after installing the committed contents at their final locations. Thus journal pins keep modifications resident after callers release them. Its eviction loop does not perform the generic dirty-victim [buffer cache writeback](#buffer-cache-writeback) of our model. [buf.h](computer-science-bibliography.md#xv6-risc-v-source-code/buf-h)[log.c](computer-science-bibliography.md#xv6-risc-v-source-code/log-c)

### Page cache

↑ **Parent:** [Buffer cache](#buffer-cache)

Caching [file](#computer-file) contents in units based on [memory pages](virtual-memory.md#memory-page), commonly by a [file](#computer-file) mapping and an offset, rather than necessarily by the device-and-block [buffer cache key](#buffer-cache-key) used above. A [file](#computer-file)'s offset must be mapped to storage before device access; the two naming systems describe different layers. How [page cache](#page-cache) and [buffer cache](#buffer-cache) storage relate depends on the [operating system](operating-system.md) and [file system](file-system.md). A separate duplicate copy at each layer is not a universal requirement.

For the [Linux kernel](operating-system.md#linux-kernel) interfaces documented in [Buffer Heads by The kernel development community](computer-science-bibliography.md#buffer-heads-by-the-kernel-development-community), per-block state can be attached to larger cached memory units called [Linux folios](#linux-folio); `mark_buffer_dirty` also marks the backing page dirty in the [page cache](#page-cache). The documented reclamation checks include dirty state, pending [buffer cache writeback](#buffer-cache-writeback) and elevated reference counts. That documentation deprecates [Linux buffer heads](#linux-buffer-head) for new [file systems](file-system.md) in favour of [iomap](#iomap). These are platform-specific interfaces, not a definition that every [page cache](#page-cache) has [Linux buffer heads](#linux-buffer-head) or that every [buffer cache](#buffer-cache) has its own disjoint allocation. [Buffer Heads by The kernel development community](computer-science-bibliography.md#buffer-heads-by-the-kernel-development-community)

#### Linux buffer head

↑ **Parent:** [Page cache](#page-cache)

The [Linux kernel](operating-system.md#linux-kernel)'s per-block state structure, which can be attached to a [Linux folio](#linux-folio). Its [reference counting](computer-science.md#reference-counting) is distinct from its dirty and valid state.

#### Linux folio

↑ **Parent:** [Page cache](#page-cache)

#### iomap

↑ **Parent:** [Page cache](#page-cache)

// Destination: computer-science.bigb

## File-system journaling

↑ **Parent:** [File system](file-system.md)

[File-system journaling](#file-system-journaling) makes a group of related [file system](file-system.md) updates recoverable after a crash by recording them in a journal before changing their final storage locations. The useful promise is [file-system crash consistency](#file-system-crash-consistency): after [journal replay](#journal-replay), a protected [file-system transaction](#file-system-transaction) has taken effect completely or has not taken effect. [File-system transaction durability](#file-system-transaction-durability) adds a different promise: an acknowledged update survives the crash. The protected group can contain only [file metadata](#file-metadata), or both [file metadata](#file-metadata) and [file data blocks](#file-data-block), depending on the [file-system journaling mode](#file-system-journaling-mode).

Consider a tiny [file](#computer-file) containing `ABCD` in four-[byte](computer-science.md#byte) [file data block](#file-data-block) 7. Its [inode](#inode) records size 4 and a reference to block 7. Appending `EFGH` in previously free block 9 requires three new stored records: $I$, the [inode](#inode) with size 8 and references to blocks 7 and 9; $B$, the [block allocation bitmap](#block-allocation-bitmap) marking block 9 allocated; and $D$, [file data block](#file-data-block) 9 containing `EFGH`. An [inode](#inode) reference to a block still marked free lets a later allocation overwrite live contents; allocating a block without recording its owner can leak space. Even mutually consistent [file metadata](#file-metadata) can expose stale contents if $D$ has not reached storage. Chapter 42 of [Crash Consistency: FSCK and Journaling](computer-science-bibliography.md#operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/crash-consistency-fsck-and-journaling) (section 42.1, pp. 2–4) develops this three-record append problem; the names, block numbers and tiny contents here are original teaching choices.

The first diagram protects all three records with [write-ahead logging](#write-ahead-logging). Each [journal payload](#journal-payload) record identifies a final destination and its complete new contents. A [storage flush](#storage-flush) makes the complete [journal payload](#journal-payload) durable before a separate [journal commit record](#journal-commit-record) is written and made durable. Only then may a [journal checkpoint](#journal-checkpoint) copy the records to their final locations. The journal remains available until those copies have themselves passed a [storage flush](#storage-flush); it can then be retired and its space reused. [Journal replay](#journal-replay) repairs an interrupted [journal checkpoint](#journal-checkpoint) using the retained new contents.[3.6. Journal (jbd2) by The kernel development community](computer-science-bibliography.md#3-6-journal-jbd2-by-the-kernel-development-community)

<a id="image-write-ahead-logging-separates-durable-journal-commit-records-from-journal-checkpoints-and-safe-journal-reuse"></a>
![](file-system-journal-transaction-timeline.png)

**[Figure 5](#image-write-ahead-logging-separates-durable-journal-commit-records-from-journal-checkpoints-and-safe-journal-reuse). Write-ahead logging separates durable journal commit records from journal checkpoints and safe journal reuse**.

These are persistence dependencies, not a claim that issuing writes in this order is sufficient. A device can report completion while its volatile [memory cache](computer-science.md#cache-computing) still holds the only copy. The [Linux kernel](operating-system.md#linux-kernel) documents both flushing earlier completed requests and making completion of a particular request depend on persistence. The timeline uses separate [storage flushes](#storage-flush) to make the dependencies explicit; an implementation can use equivalent device-supported operations. A commit write can persist before its [storage flush](#storage-flush) returns: recovery uses the actual durable marker, while acknowledgment waits for successful completion.[Explicit volatile write back cache control by The kernel development community](computer-science-bibliography.md#explicit-volatile-write-back-cache-control-by-the-kernel-development-community)

The appeal is that recovery knows exactly which updates to finish. It does not have to infer a user's intended contents from contradictory [inodes](#inode) and [block allocation bitmaps](#block-allocation-bitmap). The cost includes writing the [journal payload](#journal-payload) as well as its final copies and waiting for persistence boundaries. The journal records a recent transition, not a historical collection of recoverable [files](#computer-file); [file-system journaling](#file-system-journaling) is not a [file-system backup](#file-system-backup).

### File-system crash consistency

↑ **Parent:** [File-system journaling](#file-system-journaling)

The guarantee that recovery produces a valid [file system](file-system.md) state under a specified crash model. For the protected [file-system transaction](#file-system-transaction) in our full-data example, the observable [file](#computer-file) is either `ABCD` or `ABCDEFGH`; it never names a free block or exposes a half-applied protected append after recovery. This concerns the recovered state. The intermediate final-location records during a [journal checkpoint](#journal-checkpoint) may disagree until [journal replay](#journal-replay) finishes, and live concurrent access requires separate [synchronization](operating-system.md#synchronization-computing).

### File-system transaction

↑ **Parent:** [File-system journaling](#file-system-journaling)

A group of updates treated as one unit for [file-system crash consistency](#file-system-crash-consistency). The three-record append above is one explicitly chosen group. Real [file-system journaling](#file-system-journaling) can batch several [system calls](operating-system.md#system-call) or split large work across several groups; it does not automatically make an application's several writes into one [file-system transaction](#file-system-transaction). An [atomic operation](operating-system.md#atomic-operation) for competing [software threads](operating-system.md#thread-computing) likewise does not by itself provide [file-system transaction durability](#file-system-transaction-durability).

Creation shows why the group must include every related change. In a toy [file-system directory](#file-system-directory) with space for one more name, creating `notes` with contents `EFGH` needs a [directory entry](#directory-entry) mapping `notes` to newly allocated [inode](#inode) 42, an [inode allocation bitmap](#inode-allocation-bitmap) marking 42 in use, that [inode](#inode) with size 4 and a reference to block 9, a [block allocation bitmap](#block-allocation-bitmap) allocating 9, and [file data block](#file-data-block) 9 with the contents. An exposed [directory entry](#directory-entry) must reach an allocated [inode](#inode), and its content references must reach allocated [file data blocks](#file-data-block). Protecting just the [inode](#inode) leaves these relationships outside the [file-system transaction](#file-system-transaction). This simplified five-record creation excludes parent-directory growth, timestamps and allocation counters; a real [file system](file-system.md) must include its own additional dependencies.

#### File-system transaction durability

↑ **Parent:** [File-system transaction](#file-system-transaction)

An acknowledged [file-system transaction](#file-system-transaction) remains recoverable after a crash under the stated storage assumptions. In the full-data timeline, durable [journal payload](#journal-payload) and a durable [journal commit record](#journal-commit-record) suffice even before the [journal checkpoint](#journal-checkpoint). A crash before durable commit can lose the append while still preserving [file-system crash consistency](#file-system-crash-consistency). A successful ordinary write may only have reached a [buffer cache](#buffer-cache); an application requiring persistence must use its documented interface and check errors. On [Linux kernel](operating-system.md#linux-kernel)-based systems, [fsync](#fsync) on a [file descriptor](operating-system.md#file-descriptor) persists the associated [file](#computer-file) contents and [file metadata](#file-metadata), but persisting a newly created name also requires [fsync](#fsync) on the containing [file-system directory](#file-system-directory).[fsync(2) — Linux manual page by Linux man-pages project](computer-science-bibliography.md#fsync-2-linux-manual-page-by-linux-man-pages-project)

##### fsync

↑ **Parent:** [File-system transaction durability](#file-system-transaction-durability)

A [system call](operating-system.md#system-call) for requesting persistence of a [file](#computer-file)'s changed contents and associated [file metadata](#file-metadata). Its scope, successful completion and separate [file-system directory](#file-system-directory) synchronization matter to [file-system transaction durability](#file-system-transaction-durability).

### Write-ahead logging

↑ **Parent:** [File-system journaling](#file-system-journaling)

Making a recoverable journal entry durable before installing its protected updates at their final locations. In this article the journal contains new record images, so recovery redoes committed changes rather than undoing uncommitted changes. The diagrams assume one isolated [file-system transaction](#file-system-transaction), fresh journal slots with unambiguous record identities, no other writer, and [atomic storage writes](#atomic-storage-write) for each record and marker. A crash loses volatile state; previously durable contents remain intact. [Storage flushes](#storage-flush) are honored, and recovery finishes before the [file system](file-system.md) is exposed. These are model assumptions, not a claim that every physical [file data block](#file-data-block) write is indivisible on arbitrary hardware.

#### Journal payload

↑ **Parent:** [Write-ahead logging](#write-ahead-logging)

The protected new contents and destination information for a [file-system transaction](#file-system-transaction). In the diagrams, the three complete [journal payload](#journal-payload) records correspond to $I,B,D$. Records can reach storage in any order within this phase. The [journal commit record](#journal-commit-record) cannot become durable until all three are durable.

#### Journal commit record

↑ **Parent:** [Write-ahead logging](#write-ahead-logging)

A marker identifying a complete committed [file-system transaction](#file-system-transaction). A marker alone is insufficient if its [journal payload](#journal-payload) is missing or belongs to another group. The simple model prevents this through ordering and fresh record identities. Real journal formats also validate record identities and integrity: the [ext4](#ext4) documentation says replay discards a group lacking its commit or having mismatched integrity checks.[3.6. Journal (jbd2) by The kernel development community](computer-science-bibliography.md#3-6-journal-jbd2-by-the-kernel-development-community)

#### Journal checkpoint

↑ **Parent:** [Write-ahead logging](#write-ahead-logging)

Installing committed [journal payload](#journal-payload) at final locations and making those copies durable. Safe retirement follows this completion, not merely submission of the copies. Discarding the journal while some copies remain only in a volatile [memory cache](computer-science.md#cache-computing) can leave an unrecoverable mixture after a crash. Commit establishes a recoverable decision; a [journal checkpoint](#journal-checkpoint) permits reclamation of its journal space.

#### Journal replay

↑ **Parent:** [Write-ahead logging](#write-ahead-logging)

Reinstalling the complete new images of a committed [file-system transaction](#file-system-transaction) after a crash. An uncommitted [journal payload](#journal-payload) is ignored. Rewriting the same image has [idempotence](algebraic-operation.md#idempotence): repeating it gives the same contents, unlike performing "append four more [bytes](computer-science.md#byte)" again. If recovery itself crashes, retaining the journal until the [journal checkpoint](#journal-checkpoint) is durable allows the same recovery to restart.

The second diagram exhausts the small full-data model. A triple lists $I,B,D$ in that order; a [bit](information-theory.md#bit) is 1 exactly when the corresponding new record has persisted. Before commit, any of the $2^3=8$ [subsets](set.md#subset) of [journal payload](#journal-payload) records can be durable, while every final-location triple is `000`. After commit, the journal triple is `111`, while any of the eight final-location triples can be durable. Retirement adds one state: the live journal is gone and the final-location triple is `111`. Thus there are $8+8+1=17$ distinct abstract crash states. Waiting for a [storage flush](#storage-flush) without another record reaching persistence does not create an additional state. Retirement is modeled as an atomic change of live-log status: old payload [bytes](computer-science.md#byte) may remain physically present but are no longer part of the live journal.

<a id="image-all-17-abstract-crash-states-recover-to-the-old-or-new-three-record-append-under-the-stated-storage-flush-and-atomic-storage-write-assumptions"></a>
![](file-system-journal-crash-state-recovery.png)

**[Figure 6](#image-all-17-abstract-crash-states-recover-to-the-old-or-new-three-record-append-under-the-stated-storage-flush-and-atomic-storage-write-assumptions). All 17 abstract crash states recover to the old or new three-record append under the stated storage flush and atomic storage write assumptions**.

The short correctness argument has three cases. Before commit, final locations are unchanged. With commit, the complete [journal payload](#journal-payload) restores `111` regardless of the current final-location [subset](set.md#subset). After retirement, `111` is already durable. Each of the six partial final-location triples is repairable because its journal is retained. The enumeration is exhaustive for these records and phase rules; it excludes torn records, dishonest flush completion, media corruption, journal reuse across several [file-system transactions](#file-system-transaction) and failures of the recovery code. It is a model check, not a measured crash test of [ext4](#ext4).

### File-system journaling mode

↑ **Parent:** [File-system journaling](#file-system-journaling)

Which contents pass through the journal and which persistence dependencies accompany them. The [ext4](#ext4) documentation distinguishes these modes: [file metadata](#file-metadata) and contents both pass through the journal in `data=journal`; only [file metadata](#file-metadata) is journaled in `data=ordered`, with associated contents forced to final locations before metadata commit; only [file metadata](#file-metadata) is journaled in `data=writeback`, without that data-before-commit dependency.[ext4 General Information by The kernel development community](computer-science-bibliography.md#ext4-general-information-by-the-kernel-development-community)

For our append, full data journaling uses the three-record model. Ordered metadata journaling protects $I,B$ in the journal and first persists $D$ directly in free block 9. Before commit, changing an unreferenced free block does not change the visible old [file](#computer-file); after commit, [journal replay](#journal-replay) supplies the new [file metadata](#file-metadata) and the new contents are already durable. Without that dependency, recovery can produce correct allocation and size but stale contents in block 9. Ordered metadata journaling does not give general all-or-nothing contents for overwrites of already allocated [file data blocks](#file-data-block), nor does it combine arbitrary application writes into a [file-system transaction](#file-system-transaction). The choice of protected records determines the scope of the guarantee.

## File-system allocation bitmap

↑ **Parent:** [File system](file-system.md)

A [data structure](data-structure.md) using a [bit](information-theory.md#bit) per allocation unit to mark whether it is available. Its agreement with ownership references is a [file-system crash consistency](#file-system-crash-consistency) requirement; changing just this structure does not install the owner's update.

### Block allocation bitmap

↑ **Parent:** [File-system allocation bitmap](#file-system-allocation-bitmap)

A [file-system allocation bitmap](#file-system-allocation-bitmap) for storage blocks. In the append model, the [bit](information-theory.md#bit) for [file data block](#file-data-block) 9 changes from 0, free, to 1, allocated.

### Inode allocation bitmap

↑ **Parent:** [File-system allocation bitmap](#file-system-allocation-bitmap)

A [file-system allocation bitmap](#file-system-allocation-bitmap) for [inodes](#inode). Appending to an existing [file](#computer-file) does not allocate an [inode](#inode); creating the toy [file](#computer-file) does.

## Storage flush

↑ **Parent:** [File system](file-system.md)

A request whose successful completion, under the device's stated contract, makes preceding covered writes survive loss of volatile [memory cache](computer-science.md#cache-computing) contents. The diagrams wait for completion at each persistence boundary. [Storage flush](#storage-flush) and [atomic storage write](#atomic-storage-write) are different properties: persistence of completed writes does not make a multi-record update indivisible.

## Atomic storage write

↑ **Parent:** [File system](file-system.md)

A write whose durable result after a crash is either the complete old record or the complete new record. Its unit and failure conditions must be stated. The diagrams assume this property for each payload record, final-location record, commit marker and retirement marker; they do not derive it from the size of a [file data block](#file-data-block).

## ext4

↑ **Parent:** [File system](file-system.md)

A [Linux kernel](operating-system.md#linux-kernel) [file system](file-system.md) whose documented [file-system journaling modes](#file-system-journaling-mode) provide the implementation examples here. The diagrams specify a simpler abstract protocol, not its full on-storage format.

## File-system backup

↑ **Parent:** [File system](file-system.md)

A separately retained copy intended to recover [files](#computer-file) after loss or unwanted changes. A journal can be overwritten after a [journal checkpoint](#journal-checkpoint) and can faithfully commit an unwanted deletion; it does not supply that historical copy or protect against loss of the device holding the only copy.

// Target: computer-science.bigb

## Access control list

↑ **Parent:** [File system](file-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Access_control_list)

// Target: computer-science.bigb

## File Allocation Table

↑ **Parent:** [File system](file-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/File_Allocation_Table)

// Target: computer-science.bigb

### FAT32

↑ **Parent:** [File Allocation Table](#file-allocation-table)

// Target: computer-science.bigb

## NTFS

↑ **Parent:** [File system](file-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/NTFS)

// Target: computer-science.bigb

## Inode

↑ **Parent:** [File system](file-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inode)

An [inode](#inode) is a [data structure](data-structure.md) describing an object in an [inode](#inode)-based [file system](file-system.md). For an ordinary [file](#computer-file), it records [file metadata](#file-metadata) such as type, owner, access permissions, size and [hard link](#hard-link) count, together with information locating the contents. In the direct-reference toy layout, [inode](#inode) 42 points to [file data blocks](#file-data-block) 7 and 9; its two names `a` and `b` live in [directory entries](#directory-entry). Other [file systems](file-system.md) can locate contents differently, so the diagram is a model of the separation rather than a universal storage layout. [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 40, sections 40.3–40.4: inodes and directory organization](https://pages.cs.wisc.edu/~remzi/OSTEP/file-implementation.pdf)

An [inode](#inode) number is unique only within its [file system](file-system.md) among allocated objects. Two different [file systems](file-system.md) can each have [inode](#inode) 42, referring to unrelated [files](#computer-file). [POSIX](operating-system.md#posix) exposes the [file system](file-system.md)'s device identity as `st_dev` and the [file](#computer-file)'s serial number as `st_ino`; the pair identifies a [file](#computer-file) within a running system. Neither the bare [inode](#inode) number nor that pair is a permanent historical identifier: after reclamation, a later [file](#computer-file) can reuse the number. In particular, comparing an old saved number with a new one does not establish continuity of the [file](#computer-file). [The Open Group, POSIX.1-2017, sys/stat.h: joint identity from st\_dev and st\_ino](https://pubs.opengroup.org/onlinepubs/9699919799/basedefs/sys_stat.h.html)

The design's appeal is that one [inode](#inode) unifies the [file metadata](#file-metadata) and contents reached through several [directory entries](#directory-entry). Ritchie and Thompson's original 1974 account explicitly describes a [directory entry](#directory-entry) as a name and an i-number, with the corresponding [inode](#inode) holding ownership, protection, size, content addresses and the [hard link](#hard-link) count. It gives a concrete early explanation of how names and [file](#computer-file) identity can evolve separately. [Ritchie and Thompson, The UNIX Time-Sharing System, 1974, section 4: implementation of the file system](https://www.cs.cmu.edu/~15712/papers/ritchie74.pdf)

// Target: computer-science.bigb

## ↑ Ancestors (3)

1. [Operating system](operating-system.md)
2. [Computer science](computer-science.md)
3. [Codex Wiki](README.md)

## ← Incoming links (20)

- [Buffer cache](#buffer-cache)
- [Data compression](data-compression.md)
- [Directory entry](#directory-entry)
- [ext4](#ext4)
- [File system](file-system.md)
- [File-system crash consistency](#file-system-crash-consistency)
- [File-system directory](#file-system-directory)
- [File-system journaling](#file-system-journaling)
- [File-system transaction](#file-system-transaction)
- [Hard link](#hard-link)
- [Inode](#inode)
- [Kernel (operating system)](operating-system.md#kernel-operating-system)
- [Linux kernel](operating-system.md#linux-kernel)
- [Memory-mapped file synchronization](virtual-memory.md#memory-mapped-file-synchronization)
- [Microkernel](operating-system.md#microkernel)
- [Microkernel file-read example](operating-system.md#microkernel-file-read-example)
- [Operating system](operating-system.md)
- [Page cache](#page-cache)
- [User-space service](operating-system.md#user-space-service)
- [Write-ahead logging](#write-ahead-logging)
