# DeFi-anti-hack-checklist

As DeFi protocols advance, so do the security issues associated with them. The cost of attacking DeFi protocols has also made it clear that DeFi security needs to be emphasized. So, we have made anti-hack checklists for projects, which will help them build and develop secure DeFi applications.

**We will be actively monitoring and updating this repository. If you find anything missing or want to update existing resources, you can create a pull request and contribute to the project**

## Before Deployment:

| Serial No | Topic | Description |
| --- | --- | --- |
| 1 | **Use the latest version of Solidity/Rust** | When deploying contracts, one should use the latest released version of Solidity/Rust. This is because breaking changes, as well as new features and bug fixes, are introduced regularly. Check that your code has no reported issues with the latest compiler version. |
| 2 | **Hire experienced DeFi developers** | To ensure you develop the best DeFi project out there, make sure to hire a DeFi developer who is skilled and experienced. An experienced team of DeFi developers has accurate knowledge of DeFi project vulnerabilities and specifications. |
| 3 | **Full unit test coverage** | Unit testing improves software quality with every code check-in and build. Unit testing is the quickest, most direct way to identify and fix bugs before they influence the main codebase. An extensive test suite is crucial to building high-quality software. |
| 4 | **Proper architecture, design, and threat modeling** | Consider all possible threats before the implementation of the smart contract. During the design process, make sure certain smart contract security assumptions are taken into account. Check out [SCSVS Architecture-Design-Threat-Modelling](https://securing.github.io/SCSVS/1.2/0x10-V1-Architecture-Design-Threat-modelling.html) for more details on it. |
| 5 | **Follow well-known programming practices** | Smart contracts are developed using different programming languages such as Solidity, Vyper, Rust, etc. The development of smart contracts has proven to be extremely error-prone. It is important to follow best programming practices to develop secure code. |
| 6 | **Do thorough code documentation** | Proper source code documentation is essential for every well-maintained project. It helps the reader to understand the code better. A developer who is trying to improve the code with new features will find this very useful. The Natspec format can be used for Solidity. |
| 7 | **Make your application modular if possible** | Split the logic of the system, either through multiple contracts or by grouping similar functions together, for example, authentification, arithmetic, etc. This will facilitate easier review and allow the testing of individual components. |
| 8 | **Log all crucial operations** | Events will aid in contract debugging during development and contract monitoring after deployment. So, It is recommended to emit events for critical functions like changing owner, distribution of rewards, etc. |
| 9 | **Use the latest and well-tested libraries** | Always use the latest and well-tested libraries like openzeppelin. These libraries are well tested, and community-reviewed contracts, so they are considered more secure. For example, If we want to write an ERC20 contract, we can use OpenZeppelin. |
| 10 | **Stop Using Single Source as Price Oracle** | One of the best practices for addressing the DeFi security examples of exploits due to oracle attacks is to look for an alternative to centralized oracles. Decentralized oracles can help in finding out the true value of exchange rates, thereby ensuring better decisions for security. |
| 11 | **Make contracts Upgradable** | Smart contracts in Ethereum are immutable by default. Once we create them there is no way to alter them, effectively acting as an unbreakable contract among participants. Upgradable contracts allow us to iteratively add new features to our project, or fix any bugs or vulnerabilities missed during audits. See this [blog](https://docs.openzeppelin.com/learn/upgrading-smart-contracts#whats-in-an-upgrade) for more details on Upgradable contracts. |
| 12 | **Consider making the contract pausable** | A pausable Contract can be useful in limiting the harm done by attackers in case of an ongoing attack on the project. There are also other advantages of it. So, consider making the contract pausable. |
| 13 | **Avoid known pitfalls and common vulnerabilities** | Learn the most pitfalls and common security vulnerabilities in Solidity smart contracts and how to mitigate them. There are many online resources to learn about common issues, such as [SWC Registry](https://swcregistry.io/), [DeFi attack vectors](https://github.com/Quillhash/DeFi-Attack-Vectors), [Solidity attack vectors](https://github.com/Quillhash/Solidity-Attack-Vectors) and CTFs like [Ethernaut](https://ethernaut.openzeppelin.com/), [Capture the Ether](https://capturetheether.com/), etc. |
| 14 | **Access Control Protection for critical operations** | Hackers can easily exploit a smart contract if access control is handled poorly or not at all. So, it's very important for the protocol to implement access control protection and restrict critical functions to the owner/admin role. |
| 15 | **Design secure Tokenomics for Application** | The most crucial step in creating a token is to design its tokenomics and define product usage cases. Tokenomics modeling involves interdisciplinary aspects of mathematics, behavioral psychology, macroeconomics, game theory, game design, and related industries. Check out this [blog](https://maxya.mp/how-to-design-tokenomics-for-your-cryptocurrency-the-basics-of-creating-your-token) for more details on designing secure tokenomics. |
| 16 | **Use Automated anomaly detection tools** | It is recommended to use automated vulnerability detection tools like slither, smartcheck, etc. once we have finished writing our smart contract to eliminate all obvious vulnerabilities that may cost us so much money in the future. |
| 17 | **Perform formal verification** | Formal verification is a technique that uses exact mathematical processes to show that a design is accurate and to show where an error originated. It ensures the correctness of contracts. |
| 18 | **Smart contract audits** | Smart contract audit will help us detect uneven and unexpected vulnerabilities of smart contracts before project deployment and, therefore, prevent DeFi hacking. Smart Contract Audits Build Social Authority and it also helps in earning Users/Investors trust for the Product.

---

## After Deployment:

| Serial No | Topic | Description |
| --- | --- | --- |
| 1 | **Safeguard wallet of Privileged User** | If the private key of the admin/owner of a smart contract is leaked, all the funds and operation of the smart contract will be at great risk. Properly secure your wallet and always use a hardware wallet or a multisig wallet which is considered more secure. Check out [this](https://blog.trailofbits.com/2018/11/27/10-rules-for-the-secure-use-of-cryptocurrency-hardware-wallets/) blog for more details on wallet security. |
| 2 | **Host a bug bounty program** | Companies can enhance the protocol's security from potential hackers by running a bug bounty program. Projects can host their own bug bounty program or integrate with Bug Bounty Platforms like Immunefi or Hackerone. It adds an extra layer of security for the projects. |
| 3 | **Periodic Audits** | The periodic audits of DeFi Smart Contracts are important if the project launches any new features or updates any existing code logic. This can help the protocol fix vulnerabilities quickly before deploying to the mainnet. |
| 3 | **Insurances** | An insurance fund would greatly help alleviate damages in the event of an exploit and could set users’ minds at ease knowing that they have coverage. In case of a security incident, projects can benefit from the insurance policy to strengthen their infrastructure or reimburse the affected users. |
| 4 | **On-Chain Monitoring** | Watch the logs, and be ready to react in case of contract or wallet compromise. On-chain activity monitoring or tracking tools help in detecting critical actions, or any malicious transactions in smart contracts. These tools then notify teams through custom notifications so they can take the appropriate action as soon as possible. |
| 5 | **Disaster Recovery Plan** | Every day hacks worth millions of dollars occur. Protocols should also be on building plans for recovering from such incidents. Some of the common suggestions for a disaster recovery plan include upgrade plans or insurance. Another proven solution for disaster recovery plans includes the installation of the emergency ‘pause’ feature. |
| 6 | **Register at Rating institutions** | Add your contact info to [blockchain-security contacts](https://github.com/crytic/blockchain-security-contacts). It helps others to contact you if a security flaw is discovered. |
| 7 | **Keeping Your Tools and Devices Up to Date** | Using outdated devices and services leaves our data vulnerable to hackers. Device manufacturers and app developers will usually release software updates regularly that patch the vulnerabilities. So, regularly updating devices and tools keeps us safe from hackers.
| 8 | **Enable Authentication Methods/ 2FA to prevent Social account hacks.** | There are lots of scenarios where DeFi projects' social media accounts like Discord and Twitter are hacked, and the hackers use the compromised accounts for their personal gain. It harms the business's reputation. Using complex passwords in conjunction with 2FA enabled can thus aid in the protection of these accounts. |

In a field like blockchain, which is continually growing, the saying "security is a journey and not a destination" reminds us that we should never stop learning.

---

### References:

[https://securing.github.io/SCSVS](https://securing.github.io/SCSVS)   
[https://ethereum.org/en/developers/tutorials/smart-contract-security-guidelines/](https://ethereum.org/en/developers/tutorials/smart-contract-security-guidelines/)   
[https://101blockchains.com/top-defi-security-best-practices/](https://101blockchains.com/top-defi-security-best-practices/)
