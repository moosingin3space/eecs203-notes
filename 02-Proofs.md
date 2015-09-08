# Proofs

## What is a proof?

> A formal proof of a *proposition* is a chain of logical deductions leading
> to the proposition from a base set of axioms.

where a *proposition* is defined as a declarative statement that is either true
or false,
and an *axiom* is a proposition assumed to be true.

### Examples of propositions

- Two non-parallel lines in a plane have exactly one point in common. (True, can
  be shown to be true)
- Toronto is the capital of Canada. (False, Ottawa is the capital of Canada)
- $ 1 + 1 + 1 = 3 $ (True, assumed)

You need to define everything, and the logic cannot lead to a paradox.

## Propositional logic (propositions and connectives)

- $ \not p $ -- the opposite of p
- $ p \and q $ -- both are true
- $ p \or q $ -- at least one is true
- $ p \xor q $ -- strictly one is true
- $ p \implies q $ -- if p, then q
- $ p \iff q $ -- p if and only if q, abbreviated as "iff".

Think of the implications as nested `if` statements.

### English translations of $p \implies q$

Pattern-matching these can help a lot!

- if p then q
- p is sufficient for q
- q if p
- q when p
- q whenever p
- p implies q
- p only if q
- q follows from p
- not p unless q
- q unless not p

### Example

Convert these to math form:
1. If it rains, I'll watch a movie and eat popcorn.
2. If I don't eat popcorn, I'll eat chocolate.
3. I won't eat both chocolate and popcorn unless it rains.

1. $ r \implies (m \and p) $
2. $ \not p \implies c $
3. $ (p \and c) \implies r $

## Truth tables

|  p  |  q  | $ p \and q $ | $ p \implies q $ | $ p \iff q $ |
|:---:|:---:|:------------:|:----------------:|:------------:|
|  T  |  T  |            T |                T |            T |
|  T  |  F  |            F |                F |            F |
|  F  |  T  |            F |                T |            F |
|  F  |  F  |            F |                T |            T |
