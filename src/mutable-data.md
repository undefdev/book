# Mutable Data

> **Note:** This documentation is relevant for Flix version 0.35.0 or higher.

Flix is a _functional-first_ programming language that encourages but does not
demand, the use of immutable data structures. While immutable data structures
should be the default, Flix has rich support for imperative programming with
destructive updates to mutable data. 

Flix uses its effect system to separate pure and impure code. In particular,
Flix uses the region concept to track the use of mutable memory. That is, all
mutable memory belongs to some statically-scoped region.

Flix has two basic types of mutable memory:

- [References](./references.md)
- [Arrays](./arrays.md)

We can use references and arrays to build higher-level mutable data structures.
For example, the Flix Standard Library offers collections such as `MutList`,
`MutDeque`, `MutSet`, and `MutMap`. As a rule, these higher-level data
structures should be preferred over lower-level references and arrays.

We begin this chapter with a discussion of [regions](./regions.md).
