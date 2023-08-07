# Merkle-subset

The "Merkle-subset" is a code repository that provides functionality to generate proofs for subset Merkle trees. A subset Merkle tree proof allows you to verify whether a particular Merkle tree is a valid subset of the original Merkle tree. 

We use plonky2 library to generate proof and verify.

For example, if our original merkle tree is [a, b, c, d], some of our merkle trees are [a, 0, c, d], [a, b, 0, 0], [0, 0, 0, 0].
[x, b, c, d] is not one of our subset merkle tree.

to execute code:
```
cargo build
```

```
cargo run --example {name} --release
```

you need to use rust nightly version 

```
rustup default nightly
```
