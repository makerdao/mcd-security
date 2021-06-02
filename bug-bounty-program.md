# Bug Bounty Program

The [Bug Bounty Program](https://hackerone.com/makerdao_bbp/hacktivity?order_direction=DESC&order_field=popular&filter=type%3Abounty-awarded) is a key component of our strategy to maximize security testing by approaching it from different angles and multiple layers to ensure the security of the MCD smart contracts.

### Timeline

* Initiated the Bug Bounty program privately for selected researchers \(Private testnet on June 3rd\).
* Launched our public bug bounty program on [Hackerone](https://hackerone.com/makerdao_bbp) \(July 24th\).
* Bug Bounty Program to continue indefinitely.  

### Program Scope

The bug bounty program currently contains two separate scopes, which share the same rules with a few exceptions as noted below:

* Smart contracts for Multi-Collateral Dai.
* Infrastructure for select public facing domains \(please see the "Ineligible Bugs" section in the **Policy** section on HackerOne, especially regarding third party software, before submitting a report\).

**Note:** The program may be expanded in the future to include more asset types such as frontends and apps.

## Updates and Results

Since the launch of the program, three high-severity bugs and one critical-severity bug have been discovered, resulting in bounty reward payments totalling $90,000. The vulnerabilities consisted of unwanted interactions between the Dai Savings Rate \(DSR\) module and the Maker Protocol in one case, and the emergency shutdown module and the auctions in another case. The discoveries were in line with our expectations, as these modules either required additional scrutiny or were the most recent ones to be integrated with the system. Given that the security of the system remains our highest priority, we will continue the bug bounty program indefinitely.

