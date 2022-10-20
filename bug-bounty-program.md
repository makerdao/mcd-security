# Bug Bounty Program

Initiated early 2022, the program aims to attract whitehat hackers who find vulnerabilities and responsibly disclose them, so they are fixed before they can be exploited. Additionally, this provides an incentivized opportunity for disclosure of vulnerabilities instead of exploitation for blackhat hackers. [Immunefi Security Core Unit (ISCU)](https://mips.makerdao.com/mips/details/MIP39c2SP24#bug-bounty-program) helps run the [bug bounty program](https://mips.makerdao.com/mips/details/MIP64). Core Units need to diligently update ISCU on which assets are in-scope. ISCU will endeavour to make severity classification as objective as possible.

Two separate documents accomplish the specification of which assets are in-scope. [MIP64](https://mips.makerdao.com/mips/details/MIP64) provides the broad outlines of the program while the [Immunefi hosted document](https://immunefi.com/bounty/makerdao/) fills in the details. If there is a conflict between these two documents then MIP64 takes precedence because MIP64 was voted on by MKR holders. MIP64 provides for areas of customization that are exercised to narrow and widen the scope of the [Immunefi hosted bug bounty program](https://immunefi.com/bounty/makerdao/). Immunefi hosted bug bounty program can be modified at will by ISCU in coordination with Immunefi.

## Process

1. Whitehats create bug reports in the [Immunefi Dashboard](https://bugs.immunefi.com).
2. Immunefi Services Triaging does an initial evaluation to determine whether the report is valid.
3. ISCU is brought in to escalate bugs to the associated Maker Core Unit.
4. The associated Maker Core Unit is tasked with determining whether the report is a true vulnerability and confirm severity.
5. Optionally, for smart contract vulnerabilities, ChainSecurity can be brought in to help research bug reports.
6. If confirmed valid, ISCU will orchestrate payout of the bounty.
7. A postmortem will be published.

## Tips for Engineering Staff

- Always use the [Immunefi Dashboard](https://bugs.immunefi.com) for communications.
- Respond within 48 hours for `Critical` and `High` severity bug reports. A simple confirmation that someone is looking at the report will suffice.
- Try to close `medium/low` severity in 7 days and `high/critical` severity in 14 days.
- If you know that you will need more time, ask for it. Hackers are generally understanding, but appreciate advanced notice.
- Don't try to negotiate severity or bounty amount with the hacker. Coordinate with ISCU. :handshake: 
- If anything needs to be changed with the bug bounty program, let us know. Provide feedback. We're here to make the process work.

# Previous program

The [Hackerone](https://hackerone.com/makerdao_bbp) ran from 24 July 2019 to 2021. This program is no longer active.

## Updates and Results

Since the launch of the program, three high-severity bugs and one critical-severity bug have been discovered, resulting in bounty reward payments totalling $90,000. The vulnerabilities consisted of unwanted interactions between the Dai Savings Rate \(DSR\) module and the Maker Protocol in one case, and the emergency shutdown module and the auctions in another case. The discoveries were in line with our expectations, as these modules either required additional scrutiny or were the most recent ones to be integrated with the system. Given that the security of the system remains our highest priority, we will continue the bug bounty program indefinitely.
