PLONK Primer
============

## Design Goal and Innovation

A universal fully-succinct zk-SNARK:
 * updatable SRS
 * succint proof size
 * poly-log verification time
 * quashi-linear prover time

Innovation of PLONK:
 * a more direct arithmetization
 * a permutation argument over univariate evaluations on a multiplicative subgroup


> Note: why multiplicative subgroup is useful?
> Multiplicative subgroups are used a permutation argument based on Bayer and Groth [BG12]. Ultimately, in the “grand product argument”, this reduces to checking relations between coefficients of polynomials at “neighbouring monomials”.

TODO: understand the example in the intro - multiplicative subgroups interact well with Lagrange bases.

## A batched version of KZG

Batched polynomial commitment scheme (d-polynomial commitment scheme):
 * $gen(d)$ - a randomized algorithm that output an SRS $srs$
 * 