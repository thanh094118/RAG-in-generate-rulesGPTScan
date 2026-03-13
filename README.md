# AI-Assisted Smart Contract Vulnerability Detection

![System Architecture](architecture/gptscan_pipeline.png)

Research project extending the **GPTScan smart contract vulnerability scanner** with an AI-assisted rule generation system.  
<sub><i>base vulnerability scanner:
 <a href="https://arxiv.org/abs/2308.03314">[GPTScan]</a></i></sub>  
<sub><i>exploit data sources:
 <a href="https://defillama.com/hacks">[DeFiLlama]</a> and 
 <a href="https://hackerone.com/hacktivity">[HackerOne]</a></i></sub>

The project focuses on **automatically generating vulnerability detection rules** for smart contract analysis by combining **RAG (Retrieval-Augmented Generation)** with exploit knowledge extracted from real-world DeFi incidents.

---

## Skills & Technologies

**Security:** Smart contract vulnerability analysis, exploit pattern extraction  
**Blockchain:** Solidity contract analysis, DeFi protocol vulnerabilities  
**AI Systems:** Retrieval-Augmented Generation (RAG), LLM-assisted rule generation  
**Programming:** Python, data processing pipelines  

**Tools:** GPTScan, Slither, Python, OpenAI API

---

## Exploit Pattern Analysis

Collected and analyzed vulnerability patterns from real-world DeFi incidents:

- Reviewed public audit reports and exploit disclosures
- Extracted common vulnerability patterns from **DeFi protocol hacks**
- Built a structured knowledge base of exploit behaviors

Primary sources:
- **DeFiLlama hack database**
- **HackerOne public bug bounty reports**

---

## Rule Generation System

Designed an AI-assisted system to automatically generate vulnerability detection rules.

Key components:

- **Knowledge retrieval layer**  
  Retrieves relevant exploit cases from the dataset.

- **LLM-assisted rule generation**  
  Uses RAG to generate candidate detection rules.

- **Rule template framework**  
  Converts generated outputs into structured rules compatible with GPTScan.

---

## Integration with GPTScan

The generated rules were integrated into the **GPTScan vulnerability detection pipeline**.

Improvements include:

- Expanded vulnerability rule coverage
- Reduced manual rule engineering
- Faster iteration of detection logic

---

## Evaluation

Evaluation performed using multiple smart contract vulnerability datasets:

- **Top200 dataset**
- **Web3Bugs dataset**
- **DeFiHacks dataset**

Evaluation workflow:

1. Run baseline GPTScan detection
2. Apply AI-generated rule set
3. Compare vulnerability detection performance

Result:

- **Up to 86% improvement in vulnerability detection accuracy** through iterative rule optimization.

---

## Detected Vulnerabilities

The system focuses on detecting common **DeFi smart contract vulnerabilities**, including:

- Access control flaws
- Logic errors in state transitions
- Incorrect token accounting
- Unsafe external contract calls

---

**Objective:**  
Improve smart contract vulnerability detection by combining **LLM-assisted rule generation** with **existing program analysis techniques from GPTScan**.

---

![security-research](https://img.shields.io/badge/type-security_research-red)
![smart-contract](https://img.shields.io/badge/focus-smart_contract-blue)
![ai](https://img.shields.io/badge/ai-rag_assisted-orange)
![web3](https://img.shields.io/badge/domain-web3_security-green)
