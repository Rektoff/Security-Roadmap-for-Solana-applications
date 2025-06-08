## ⚫️ Solana Application Security Roadmap

![Group 48096155](https://github.com/Rektoff/Security-SoK-for-Solana-blockchain-/assets/144442822/cb98a230-3f65-4173-9b7c-eba843cb567b)


We created a special cybersecurity Systematization of Knowledge for Solana applications and protocols. We call it the Solana Security Strategy: a database that would be hugely beneficial for anyone who wants to secure their product and learn how to approach security strategy from the best-collected resources.

If you are looking to get a personalized security roadmap developed for your Solana application - schedule a meeting with [Rektoff](https://www.rektoff.xyz/) today: [https://cal.com/rektoff](https://cal.com/rektoff)

## ⚫️ Security Strategy Overview

We've mapped security strategy into 3 main stages:

1. [**Design & Development Stage**](#%EF%B8%8F-i-design--development-stage)
2. [**Pre-deployment / Testnet Stage**](#%EF%B8%8F-ii-pre-deployment--testnet-stage)
3. [**Post-deployment / Monitoring Stage**](#%EF%B8%8F-iii-post-deployment--monitoring-stage)

---

## ⚫️ I. Design & Development Stage

### Protocol Documentation

Solana's account-based programming model introduces unique attack surfaces where malicious actors can inject arbitrary accounts into transactions. Comprehensive protocol documentation must explicitly:

- **Map all privileged roles and their associated permissions**
  - [Can You Pass the Rekt Test?](https://blog.trailofbits.com/2023/08/14/can-you-pass-the-rekt-test/)
  - [Solana Program Security Part 1](https://research.kudelskisecurity.com/2021/09/15/solana-program-security-part1/)

- **Identify and list dependencies on external services** (e.g., price oracles, cross-chain bridges)

- **Specify validation checks for:**
  - Account ownership via `AccountInfo::is_signer`
  - Data structure integrity using Anchor's type constraints
  - Cross-program invocation (CPI) authority delegation risks

### Organizational Security

- **ALWAYS conduct identity verification + background checks on all of your employees**
  - [DOJ Seeks Forfeiture of $7.7 Million in Cryptocurrency Tied to North Korean IT Worker Laundering Network](https://www.trmlabs.com/resources/blog/doj-seeks-forfeiture-of-7-7-million-in-cryptocurrency-tied-to-north-korean-it-worker-laundering-network)

- **Define a team member who will be responsible for security operations**

- **Conduct Social Engineering resistance training and tests with simulated phishing campaigns** (remember, humans are often one of the most vulnerable parts of any system)
  - [Social Engineering Training](https://hoxhunt.com/blog/social-engineering-training)
  - [Top 7 Social Engineering Frauds in Crypto](https://hacken.io/discover/top-7-social-engineering-frauds-in-crypto/)
  - [How Social Engineering Attack led to $600M+ in losses](https://rekt.news/big-phish)
  - [Train engineers on Solana-specific threats](https://ackee.xyz/solana-auditors-bootcamp)

### DevSecOps Pipeline + Operational Security

- **Hardware keys for production systems**
  - [Best Hardware Securit Keys](https://www.pcmag.com/picks/best-hardware-security-keys)
  - Use Semi-Airgapped Device (This explainw what an airgap device is: [AIRGAP Device](https://bitcoinmagazine.com/technical/why-use-an-air-gapped-computer-bitcoin)) - A Semi-Airgapped device is a device that can connect to network when needed and that does not have any app installed other than the ones intended for production work.

- **Secure your social media accounts against sim-swap and other attacks:**
  - [Discord Security by OfficerCIA](https://officercia.mirror.xyz/x4nGX6YwhhmHj8TaQ53kBR5b5M1Ei_Y9_l1Vpext-Hk)
  - [Twitter Security Self-Audit](https://securityalliance.notion.site/Twitter-Security-Self-Audit-8fdb80d93a144dbab0f0cc4ff59c2131)
  - [Telegram Security Self-Audit](https://securityalliance.notion.site/Telegram-Security-Self-Audit-863507aa2ea84360be8e6f30c61e6b0d)
  - [Google Security Self-Audit](https://securityalliance.notion.site/Google-Security-Self-Audit-6718ff76812f4be5a0e62141c66fa5ec)

- **Multi-person integrity security policy (MPC / Multisig)** to eliminate single point of failure:
  - [Squads Multisig](https://squads.xyz/squads-multisig)

- **Solana Assets Security:**
  - [Slowmist: Exploring Solana - A Comprehensive Guide to Accounts, Tokens, Transactions, and Ensuring Asset Security](https://defihacklabs.substack.com/p/exploring-solana-a-comprehensive)

### Internal Security Testing

- **Automated Scanning**
  - [How to Audit Solana Smart Contracts Part 2: Automated Scanning](https://www.sec3.dev/blog/how-to-audit-solana-smart-contracts-part-2-automated-scanning)

- **Solana Fuzz Testing**
  - [Trident](https://github.com/Ackee-Blockchain/trident)
  - [Honggfuzz-rs](https://github.com/rust-fuzz/honggfuzz-rs#how-to-use-this-crate)
  - [Rust Fuzzers](https://docs.ziion.org/discover-the-tools/rust-fuzzers)
  - [Lessons from fuzzing a smart contract compiler](https://www.youtube.com/watch?v=8E7XOHQiRPE)
  - The [Helius Security Guide](https://www.helius.dev/blog/a-hitchhikers-guide-to-solana-program-security) emphasizes boundary condition testing for program-derived addresses (PDAs), as incorrect `find_program_address` usage can lead to seed collisions. Implement fuzz testing early using tools like [Trident](https://github.com/Ackee-Blockchain/trident) to simulate adversarial inputs

- **Other SAST / DAST on every commit**
  - [Rust Tools](https://docs.ziion.org/discover-the-tools/rust-tools) and [Automated Tools](https://docs.ziion.org/discover-the-tools/rust-automated-tools)

---

## ⚫️ II. Pre-deployment / Testnet Stage

The pre-deployment stage is a pivotal checkpoint in a protocol's journey to mainnet. It's the point where theoretical risks meet practical implementation. Where undetected flaws can become multimillion-dollar vulnerabilities. At this stage, security should be proactive, layered, and aligned with the protocol's architecture. This includes threat modeling, fuzzing campaigns, formal verification, and security reviews. Rather than relying on a last-minute audit alone, teams should design security into their development cycle, ensuring their system is resilient before it ever touches users or capital.

If you're aiming to embed security into every stage of your development lifecycle, we encourage you to [reach out](https://cal.com/rektoff). Our distributed network of top-tier security engineers offers comprehensive support across the entire engineering process. By streamlining your security strategy and applying our deep experience, we help reduce operational risk, so your team can stay focused on building and scaling with confidence.

### External Security Testing

- **Begin scheduling security reviews at least 8 weeks before your planned launch date**

- **Keep in mind:** the effectiveness of a security audit is directly tied to your audit readiness. To get the most value from the review, we strongly recommend [passing an audit readiness checklist](https://amp.runtimeverification.com/readiness-guide) beforehand

- **Fuzzing as a Service**
  - using [Trident](https://github.com/Ackee-Blockchain/trident) 

- **Schedule an audit contest**

- **Web app audit / pentesting**

- **Stress Testing**

- **Formal Verification**
  - [Certora Solana Prover](https://docs.certora.com/en/latest/docs/solana/index.html)
  - [Formally Verifying Solana Programs by OtterSec](https://osec.io/blog/2023-01-26-formally-verifying-solana-programs)
  - [Formal Verification of Solana Smart Contracts by Certora](https://medium.com/certora/formal-verification-of-solana-smart-contracts-2e57b960f953)

### Security Reviews

**The most expert teams for Solana-based security reviews:**

- [Runtime Verification](https://runtimeverification.com/)
- [OtterSec](https://osec.io/)
- [Neodyme](https://neodyme.io/en/)
- [Sec3](https://www.sec3.dev/)
- [Zellic](https://www.zellic.io/)
- [Ackee Blockchain](https://ackee.xyz/)
- [Hexens](https://hexens.io/)
- [Trail of Bits](https://www.trailofbits.com/)
- [Kudelski Security](https://kudelskisecurity.com/)
- [Cantina](https://cantina.xyz/)
- [Certora](https://www.certora.com/)
- [Sherlock](https://www.sherlock.xyz/)
  
---

## ⚫️ III. Post-deployment / Monitoring Stage

The post-deployment stage is the time to improve, analyze, and prepare for emergent situations. It's critically important to understand that no defensive solution can guarantee 100% protection of your blockchain software against hacker activities. Your team should be prepared to respond reactively to prevent disasters swiftly. Developing an Incident Response Plan (IRP), launching bug bounty (BB), and integrating advanced on-chain monitoring technology with supportive SOC analysts can significantly improve outcomes in the event of malicious incidents.

You should never stop thinking about security. It is essentially a repetitive process. Even if your project has significantly evolved in reputational and operational maturity, continuous 24/7 analysis and monitoring remain mandatory.

### Key Activities

- **Launching a bug bounty program**
  - [Why your web3 project needs a bug bounty program](https://consensys.io/diligence/blog/2023/06/why-your-web3-project-needs-a-bug-bounty-program/)
  - [How to get started with bug bounties by OWASP](https://owasp.org/www-chapter-czech-republic/slides/Getting_Started_with_Bug_Bounty.pdf)

- **Incident Response Plan development**
  - [Crisis Handbook during smart contract hacks](https://docs.google.com/document/d/1DaAiuGFkMEMMiIuvqhePL5aDFGHJ9Ya6D04rdaldqC0/edit#heading=h.mu60v0fbgnvg) - This was tailored for EVM but most of the 

- **Onchain Monitoring integration + SOC center 24/7 support**
  - [Watchtower by Sec3](https://www.sec3.dev/watchtower)
  - [Transaction simulation by Range Security](https://www.range.org/transaction-security)
  - [Onchain monitoring by Blockaid](https://blockaid.io/platform)

- **Ongoing security reviews and formal verification for each new update/integration**

---

## ⚫️ Strengthening

Do not think of security as a timestamp before deployment. When building financial infrastructure, security must be a way of thinking, writing code, managing teams, and scaling systems.
At Rektoff, we’re restructurinng approach to security by embedding it across the entire engineering lifecycle. Through a distributed network of elite engineers and Rust security specialists, we make high-impact security knowledge, workflows, and tools accessible to every team - no matter their size or stage.

Stay [Rektoff](https://linktree.com).
