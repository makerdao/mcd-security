# MCD Security Audits

We determined that the best strategy to maximize security would be to combine our formal verification efforts with more traditional security audits paired with higher-level formal modeling. Therefore, we partnered with three leading independent security auditors to protect against logical errors and/or potential failure modes in the contract logic. 

**The following industry experts focused on:** 
- **[Trail of Bits](https://www.trailofbits.com/)** - security reviews of our smart contracts. 
- **[PeckShield](https://peckshield.com/)** - traditional audit. 
- **[Runtime Verification](https://runtimeverification.com/smartcontract/)** - creating a high-level formal model that can be used to further verify the logic of the system.

# Updates and Results

### Runtime Verification Update

Runtime Verification, an Illinois-based software analysis company, uses runtime verification-based techniques to improve the safety, reliability, and technical “correctness” of software systems. The Runtime Verification team has completed its high-level model of the core MCD system and has begun building models of the other modules. The team expects to complete their work late this fall, likely by the end of November. 

### [Trail of Bits Final Audit Report](https://github.com/makerdao/mcd-security/blob/master/Audit%20Reports/TOB_MakerDAO_Final_Report.pdf)

Trail of Bits (ToB), a world leader in security, has audited our MCD smart contracts. ToB reviews a broad variety of software, creates security tooling, and consults on the modifications necessary for secure system deployment. Its audit consisted of manual review, automated analysis, and bespoke tool development. 

**Summary of Findings**
- The Trail of Bits team identified two medium-severity issues, four low-severity issues, and eight informational security issues.
- In its audit report, the ToB team noted that our use of formal verification eliminated much of the “low-hanging fruit” in terms of vulnerabilities, and recommended continued use.
- The ToB team also developed several security analysis tools specialized to the MCD codebase. These tools were used throughout the course of the audit to discover bugs, and then delivered to the MCD team once the audit was completed.
- ToB had one specific finding concerning the DSR that we want to address here ([source](https://github.com/makerdao/mcd-security/blob/master/Audit%20Reports/TOB_MakerDAO_Final_Report.pdf), pp. 22). We understand the perceived issue and are exploring the possibilities of how we could apply the DSR to Dai throughout the system. In the meantime, we agree with the risks of users' non-standard ERC-20 proxies for the DSR and have begun R&D on a proof-of-concept implementation. As always, we recommend users practice caution when using third-party smart contracts to interact with the MCD system.
- [Final Audit Report](https://github.com/makerdao/mcd-security/blob/master/Audit%20Reports/TOB_MakerDAO_Final_Report.pdf)

### [PeckShield Final Audit Report](https://github.com/makerdao/mcd-security/blob/master/Audit%20Reports/PeckShield_Final_Audit_Report.pdf) 

PeckShield, a security services organization based in China, had previously and independently verified the Maker DSChief vulnerability that was patched in May. Therefore, we contracted them to do a formal audit. 

**Summary** 
- The PeckShield team identified one high-severity issue (previously discovered through the bug bounty program), one medium-severity issue, four low-severity issues, and 10 informational security issues.
- In its audit report, the team recognized our independent security efforts: “We always recommend proceeding with several independent audits and a public bug bounty program to ensure the security of smart contract(s).” 
- Zero bugs noted in PeckShield’s “17 Typical Smart Contract Coding Bugs” list were found. 
- [Final Audit Report](https://github.com/makerdao/mcd-security/blob/master/Audit%20Reports/PeckShield_Final_Audit_Report.pdf)

### Third-Party Audit Results

In addition to the audit results provided by the three contracted organizations noted above, we were contacted by a third-party security firm, Certora, who presented findings after reviewing the MCD code on their own and with their own tools. We want to thank Certora for independently verifying two important vulnerabilities.


## In Summary 

**Overall, security audits have covered the following areas within MCD:**
- The core Maker Protocol
- Incentive reasoning
- DoS, Replay, Front-running, System/Blockchain-level attacks 
- Governance Attacks
- Governance (general)
- Front-end contracts and collateral adapters
- Oracles
- Off-chain price-feed infrastructure
- On-chain oracle contracts
- System deployment and Permissions correctness
- Auctions
- K-dss


Our efforts from all four security tracks have resulted in the discovery of a number of bugs, including some high- and critical-severity issues. We’ve taken steps to evaluate and mitigate these issues, and we will continue to work with auditors to verify that we have completely addressed them pre-MCD launch. 
