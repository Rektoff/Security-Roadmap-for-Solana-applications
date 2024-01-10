# Solana dApp Security Roadmap
### Security SoK(Systematization of Knowledge) for Solana applications

![Group 48096155](https://github.com/Rektoff/Security-SoK-for-Solana-blockchain-/assets/144442822/cb98a230-3f65-4173-9b7c-eba843cb567b)


We decided to create a special cybersecurity Systematization of Knowledge for Solana applications and protocols. We call it the Solana Security Strategy: such a database would be hugely beneficial for anyone who wants to secure their product and learn security from the best-collected resources.

If you are looking to get a personalized security strategy developed for your Solana application- schedule a meeting with [Rektoff](https://www.rektoff.xyz/) today: [https://app.reclaim.ai/m/gregory-makodzeba/flexible-meeting](https://app.reclaim.ai/m/gregory-makodzeba/flexible-meeting)

### We’ve mapped the cybersecurity strategy into 3 main stages:
1. ## **Design & Development stage**
2. ## **Pre-deployment / Testnet stage**
3. ## **Post-deployment / Monitoring stage**

----------------

### I. Design & Development stage

- **Protocol Documentation**
  - Document the system’s Access Control / Privileges / Roles 
    - [https://blog.trailofbits.com/2023/08/14/can-you-pass-the-rekt-test/](https://blog.trailofbits.com/2023/08/14/can-you-pass-the-rekt-test/)
    - [https://research.kudelskisecurity.com/2021/09/15/solana-program-security-part1/](https://research.kudelskisecurity.com/2021/09/15/solana-program-security-part1/)
  - Document all external services, contracts and oracles your application relies on 
  - Document all of the potential attack vectors on your system
    
- **Organizational security**
  - ALWAYS conduct identity verification + background checks on all of your employees
    - [https://www.mandiant.com/resources/blog/lightshow-north-korea-unc2970](https://www.mandiant.com/resources/blog/lightshow-north-korea-unc2970)
  - Define a team member who will be responsible for security operations 
  - Conduct Social Engineering training and tests (remember, humans are often one the most vulnerable parts of any system)
    - [https://blog.knowbe4.com/cisco-web-3.0-will-be-the-next-frontier-for-social-engineering-and-phishing-attacks](https://blog.knowbe4.com/cisco-web-3.0-will-be-the-next-frontier-for-social-engineering-and-phishing-attacks)
      
- **DevSecOps pipeline + Operational Security**
  - Hardware keys for production systems
    - [https://www.yubico.com/ca/product/yubikey-5-series/yubikey-5c-nano/](https://www.yubico.com/ca/product/yubikey-5-series/yubikey-5c-nano/)
  - Secure your system against sim-swap attacks:
    - Twitter security self-audit: [https://securityalliance.notion.site/Twitter-Security-Self-Audit-8fdb80d93a144dbab0f0cc4ff59c2131](https://securityalliance.notion.site/Twitter-Security-Self-Audit-8fdb80d93a144dbab0f0cc4ff59c2131)
    - Telegram security self-audit: [https://securityalliance.notion.site/Telegram-Security-Self-Audit-863507aa2ea84360be8e6f30c61e6b0d](https://securityalliance.notion.site/Telegram-Security-Self-Audit-863507aa2ea84360be8e6f30c61e6b0d)
    - Google security self-audit: [https://securityalliance.notion.site/Google-Security-Self-Audit-6718ff76812f4be5a0e62141c66fa5ec](https://securityalliance.notion.site/Google-Security-Self-Audit-6718ff76812f4be5a0e62141c66fa5ec)
  - Multi-person integrity security policy (MPC / Multisig) to eliminate single point of failure:
    - [https://squads.so/](https://squads.so/)
  - Solana Assets Security:
    - (DefiHacksLabs Exploring Solana: A Comprehensive Guide to Accounts, Tokens, Transactions, and Ensuring Asset Security)(https://defihacklabs.substack.com/p/exploring-solana-a-comprehensive)
      
- **Internal security testing**
  - Automated Scanning
    - [https://www.sec3.dev/blog/how-to-audit-solana-smart-contracts-part-2-automated-scanning](https://www.sec3.dev/blog/how-to-audit-solana-smart-contracts-part-2-automated-scanning)
  - Solana Fuzz testing
    - [https://github.com/Ackee-Blockchain/trdelnik](https://github.com/Ackee-Blockchain/trdelnik)
    - [https://github.com/rust-fuzz/honggfuzz-rs#how-to-use-this-crate](https://github.com/rust-fuzz/honggfuzz-rs#how-to-use-this-crate)
    - [https://docs.ziion.org/discover-the-tools/rust-fuzzers](https://docs.ziion.org/discover-the-tools/rust-fuzzers)
    - [https://www.youtube.com/watch?v=8E7XOHQiRPE](https://www.youtube.com/watch?v=8E7XOHQiRPE)
  - other SAST / DAST on every commit
    - [https://docs.ziion.org/discover-the-tools/rust-tools](https://docs.ziion.org/discover-the-tools/rust-tools)
    - [https://docs.ziion.org/discover-the-tools/rust-automated-tools](https://docs.ziion.org/discover-the-tools/rust-automated-tools)

### II. Pre-deployment / Testnet stage
The pre-deployment stage is one of the most critical phases, during which teams often start to involve security partners, such as Rektoff, in their processes before launching. This stage requires intensive security practices, including multi-layered reviews, penetration & stress testing, and formal verification, to ensure everything is thoroughly solid for the mainnet and interactions with users.

We recommend contacting us if you are looking to make security foundational and integrate it into every development stage. We provide full engineering lifecycle support with the best cybersecurity specialists from our distributed network. By efficiently managing your security procedures and leveraging our extensive experience, we alleviate your protocol challenges, allowing you to focus on building and accelerating your project.

- **External Security Testing**
  - Choosing security providers & scheduling security review
  - Passing audit Readiness Checklist
  - Fuzzing as a service
    - [https://arxiv.org/pdf/2309.03006v2.pdf](https://arxiv.org/pdf/2309.03006v2.pdf)
    - [https://github.com/Ackee-Blockchain/trdelnik](https://github.com/Ackee-Blockchain/trdelnik)
  - Passing an audit contest
  - Web app audit / pentesting
  - Stress Testing
  - Formal Verification
    - [https://osec.io/blog/2023-01-26-formally-verifying-solana-programs](https://osec.io/blog/2023-01-26-formally-verifying-solana-programs)
    - [https://medium.com/certora/formal-verification-of-solana-smart-contracts-2e57b960f953](https://medium.com/certora/formal-verification-of-solana-smart-contracts-2e57b960f953)
      
- **Security Review**
  - The most expert companies for Solana-based security reviews:
    - [Rektoff](https://www.rektoff.xyz/)
    - Sec3
    - Zellic
    - Ackee Blockchain
    - OtterSec
    - Hexens
    - Trail of Bits
    - Kudelski Security

### III. Post-deployment / Monitoring stage
The post-deployment stage is the time to improve, analyze, and prepare for emergent situations. It’s critically important to understand that no defensive solution can guarantee 100% protection of your blockchain software against hacker activities. Your team should be prepared to respond reactively to prevent disasters swiftly. Developing an Incident Response Plan (IRP), launching bug bounty (BB), and integrating advanced on-chain monitoring technology with supportive SOC analysts can significantly improve outcomes in the event of malicious incidents.

You should never stop thinking about security. It is essentially a repetitive process. Even if your project has significantly evolved in reputational and operational maturity, continuous 24/7 analysis and monitoring remain mandatory.

- Launching a bug bounty program
  - [https://consensys.io/diligence/blog/2023/06/why-your-web3-project-needs-a-bug-bounty-program/](https://consensys.io/diligence/blog/2023/06/why-your-web3-project-needs-a-bug-bounty-program/)
- Incident Response Plan development
  - [https://docs.google.com/document/d/1DaAiuGFkMEMMiIuvqhePL5aDFGHJ9Ya6D04rdaldqC0/edit#heading=h.mu60v0fbgnvg](https://docs.google.com/document/d/1DaAiuGFkMEMMiIuvqhePL5aDFGHJ9Ya6D04rdaldqC0/edit#heading=h.mu60v0fbgnvg)
- Onchain Monitoring integration + SOC center 24/7 support 
  - [https://www.sec3.dev/watchtower](https://www.sec3.dev/watchtower)
- On-going security reviews and verifications for each new update/integration

### Strengthening:

As a result of the behaviour previously discussed, we deeply believe that security systems can enhance any blockchain, protocol, or application at any stage of its development roadmap. The primary value Rektoff focuses on is bringing accessible security knowledge, practices, and support to everyone in the market through a distributed network of engineers and security talents, which are integral to our company and its key solutions.

In the case of Solana, we have the opportunity to redefine DevOps processes and evolve them into a more advanced DevSecOps type of operation. By learning from existing attack vectors and shared experiences in DeFi, we are confident that our customized hybrid strategy will significantly improve the performance of engineering teams in the market.

DM us to schedule an Onboarding Security Test and consultation, and refer to the information provided below for more details about our solutions:

[Rektoff Solutions](https://rektoff.notion.site/Rektoff-xyz-06d59fbfbb29429693486e25748baa76)

Stay Rektoff!
