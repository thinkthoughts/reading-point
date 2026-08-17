# Modulo 30 Reading Point

**The modular reading space stays 30 states.**

An integer can become arbitrarily large while its residue modulo 30 remains one of only 30 possible values:

`{0, 1, 2, ..., 29}`

The Modulo 30 Reading Point instrument makes that reduction visible.

Enter any integer `n`. The instrument computes:

`n mod 30`

and places the result in the 30-state modular reading space.

Eight of those states are coprime to 30:

`{1, 7, 11, 13, 17, 19, 23, 29}`

These are the reduced residue classes modulo 30.

Every prime greater than 5 occupies one of these eight classes. Composite integers may occupy them as well.

For example:

`237642387425387 mod 30 = 17`

The magnitude of the integer is large. Its modular reading remains a single state:

`17`

Because `17` is coprime to 30:

`gcd(237642387425387, 30) = 1`

so the integer is immediately excluded from divisibility by 2, 3, and 5.

The highlighted reading therefore means:

**coprime to 30**

rather than:

**prime**

## Reading the instrument

The ring displays the eight reduced residue classes:

`1 · 7 · 11 · 13 · 17 · 19 · 23 · 29`

Where the entered integer occupies one of these classes, that position is highlighted.

Where its residue is one of the other 22 states, the center still reports the exact value of `n mod 30`, while no reduced-residue position is highlighted.

This separates two mathematical objects:

**30-state modular space**

`{0, 1, 2, ..., 29}`

**8-state reduced residue system**

`{1, 7, 11, 13, 17, 19, 23, 29}`

## Reading Point

The instrument is a small example of the Reading Point approach:

**large object → specified transformation → smaller readable state**

Here the transformation is exact:

`n → n mod 30`

Magnitude changes.

**The modular reading space stays 30 states.**
