# MCD Security Audits

We determined that the best strategy to maximize security would be to combine our formal verification efforts with more traditional security audits paired with higher-level formal modeling. Therefore, we partnered with three leading independent security auditors to protect against logical errors and/or potential failure modes in the contract logic. 

**The following industry experts focused on:** 
- **[Trail of Bits](https://www.trailofbits.com/)** - security reviews of our smart contracts. 
- **[PeckShield](https://peckshield.com/)** - traditional audit. 
- **[Runtime Verification](https://runtimeverification.com/smartcontract/)** - creating a high-level formal model that can be used to further verify the logic of the system.

# Updates and Results

### Runtime Verification Update
- The Runtime Verification team has completed its high-level model of the core MCD system and has begun building models on 
the other modules.  We expect this work to be completed this fall (estimated to be concluded at the beginning of November). 

### Trail of Bits Final Audit Report 
- Identified 2 medium-severity issues, 4 low-severity issues, and 8 informational security issues.
- The ToB team directly mentions in their audit report that our team’s use of formal verification eliminated much of the “low-hanging fruit” in terms of vulnerabilities, and they recommend its continued use.
- Trail of Bits had one finding concerning the DSR. We understand the perceived issue and have come to the conclusion that we do not believe making “locking” more meaningful is the correct direction that the system should use. We are exploring possibilities in the future of applying the DSR to Dai throughout the system and thereby removing the need for locking, but this will require an "upgrade" and will have to be proposed and debated through the Governance process. In the meantime, we agree with the risks of users' non-standard ERC-20 proxies for the DSR and have begun R&D on a Proof of Concept (POC) implementation. As always we recommend users practice caution when using 3rd party smart contracts to interact with the MCD system.
- [Final Audit Report](https://github.com/makerdao/mcd-security/blob/master/Audit%20Reports/TOB_MakerDAO_Final_Report.pdf)

### Peckshield Final Audit Report 
- Identified 1 high-severity issue, 1 medium-severity issue, 4 low-severity issues, and 10 informational security issues.
- 0 bugs found from Peckshield’s “17 Typical Smart Contract Coding Bugs” list. 
- [Final Audit Report](https://github.com/makerdao/mcd-security/blob/master/Audit%20Reports/PeckShield_MakerDAO_Final_Report.pdf)

## In Summary 

**To summarize, the overall efforts of the security audits have covered the following areas:**
- The DSS System
- Incentive reasoning
- DoS, Replay, Front-running, System/Blockchain-level attacks 
- Governance Attacks
- Governance (general)
- Front-end contracts & collateral adapters
- Oracles
- Off-chain price-feed infrastructure
- On-chain oracle contracts
- System deployment & Permissions correctness
- K-dss

With respect to the audit results from Trail of Bits and Peckshield, we have already taken the necessary steps to evaluate and mitigated the issues we felt were necessary pre-launch. In addition to the 3 auditors’ findings, we were contacted by 3rd party security firms, such as Certora who have been reviewing the MCD code with their own tools and reporting their own great findings. Certora verified two issues through its own formal verification measure. We will continue to work with the auditors to verify that our mitigation efforts have completely addressed the important issues. 
