# Formal Verification

Overall, the MCD system's core contracts have been fully formally verified, and the verification of peripheral and helper contracts is ongoing. We are now currently working on the formal verification of the tokens that may be voted in as new collateral types, focusing on formally verifying the secondary contracts as well as the governance contracts in the system, and have incorporated formal verification into our continuous testing and release processes. In terms of our in-house efforts, we are leveraging klab, KEVM, and the K Framework for our Formal verification processes.

**Small-step semantics:**

* DSS Core - executable specification
* Exhaustive reachability claims
* EVM bytecode performs as we expect
* Function-level correctness
* Transaction-level correctness

**Big-step semantics:**

* Maker DSL / State Machine
* High-level system model \(K\)
* System-level invariants
* Exhaustive behaviour checking
* Executable system documentation

**Update - Formal Verification that has been completed thus far:**

* Core system
* Dai token contract
* Auction contracts
* Dai Savings Rate \(DSR\)
* Emergency shutdown module \(ESM\)
* The Oracle security module \(OSM\) has been largely completed.

Overall, the plan is to continue our formal verification efforts on the road to launching MCD, which includes updating past proofs based on the findings of our audits and bug findings.

