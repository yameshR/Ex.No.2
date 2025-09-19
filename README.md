# EX-02-Cross-Platform-Prompting-Evaluating-Diverse-Techniques-in-AI-Powered-Text-Summarization

## AIM
To evaluate and compare the effectiveness of prompting techniques (zero-shot, few-shot, chain-of-thought, role-based) across different AI platforms (e.g., ChatGPT, Gemini, Claude, Copilot) in a specific task: text summarization.

### REG.NO: 212222220059
### NAME: YAMESH R

## Scenario:
You are part of a content curation team for an educational platform that delivers quick summaries of research papers to undergraduate students. Your task is to summarize a 500-word technical article on "The Basics of Blockchain Technology" using multiple AI platforms and prompting strategies.

Your goal is to determine which combination of prompting technique + platform provides the best summary in terms of:

Accuracy

Coherence

Simplicity

Speed

User experience

## Algorithm

1. **Article Selection**
   Select a \~500-word technical article titled *"The Basics of Blockchain Technology"*.
````
The Basics of Blockchain Technology

In recent years, blockchain technology has gained significant attention for its potential to revolutionize industries beyond its original use in cryptocurrencies like Bitcoin. At its core, blockchain is a decentralized, distributed ledger system that securely records transactions across a network of computers. What makes blockchain unique is its ability to ensure transparency, security, and immutability without the need for a central authority.

What is Blockchain?

A blockchain can be thought of as a chain of digital “blocks,” each containing a record of transactions. These blocks are linked together in chronological order using cryptographic techniques. Once a block is added to the chain, the information inside it cannot be altered without changing all subsequent blocks, making the system resistant to tampering or fraud.

Key Features of Blockchain

Decentralization – Traditional databases are usually controlled by a central entity, but blockchain distributes the ledger across many nodes (computers). Every participant in the network has a copy of the blockchain, ensuring no single point of failure.

Transparency – Transactions recorded on the blockchain are visible to all participants. While identities can remain anonymous, the transaction history is permanent and accessible, which helps build trust.

Immutability – Once data is recorded on a blockchain, it cannot be changed or deleted. This permanence reduces the risk of fraud and enhances accountability.

Security – Blockchain uses cryptographic algorithms to secure transactions and control access. Each block is connected to the previous one using a unique hash, making it extremely difficult to alter data.

How Blockchain Works

When a transaction occurs, it is verified by participants in the network through a process called consensus. Different blockchains use different consensus mechanisms, such as Proof of Work (PoW) or Proof of Stake (PoS). Once verified, the transaction is grouped into a block, which is then added to the chain in a way that ensures it cannot be modified without network-wide agreement.

Applications of Blockchain

While blockchain is best known for enabling cryptocurrencies, its applications extend to many fields:

Finance – Beyond digital currencies, blockchain can streamline cross-border payments, reduce fraud, and increase transparency in banking.

Supply Chain Management – Companies can track goods from origin to destination, ensuring authenticity and reducing counterfeiting.

Healthcare – Patient records can be securely stored and shared across providers while maintaining privacy and accuracy.

Voting Systems – Blockchain-based voting can increase transparency, reduce fraud, and enhance trust in democratic processes.

Smart Contracts – These are self-executing contracts with conditions directly written into code, enabling automated and trustless transactions.

Challenges in Blockchain

Despite its advantages, blockchain faces several challenges. Scalability remains an issue, as processing a large number of transactions can be slow and energy-intensive, especially in PoW systems. Regulatory uncertainties and concerns about data privacy also pose hurdles to widespread adoption. Additionally, while immutability is a strength, it can also be a weakness if incorrect or fraudulent data is entered into the system.

Conclusion

Blockchain technology represents a transformative shift in how data and transactions are managed. By combining decentralization, transparency, and security, it has the potential to disrupt industries ranging from finance to healthcare. However, challenges related to scalability, regulation, and energy consumption must be addressed before blockchain can achieve its full potential. As research and innovation continue, blockchain is likely to become a foundational technology for the digital future.
````

3. **Prompting Strategies Definition**
   Prepare the following four prompting strategies:

   * **Zero-shot**: Directly ask the model to summarize without examples.
   * **Few-shot**: Provide 2–3 examples of summaries for similar technical texts before asking for the summary.
   * **Chain-of-Thought**: Prompt the model to explain or break down the text logically before summarizing.
   * **Role-based**: Instruct the model to act as a specific role (e.g., “a university professor summarizing for freshmen”).

4. **Platform Selection**
   Use the following AI platforms:

   * ChatGPT (OpenAI)
   * Gemini (Google)
   * Claude (Anthropic)
   * Copilot (Microsoft)

5. **Execution**
   For each platform:

   * Apply each prompting strategy using the same input article.
   * Record the output summary.
   * Note time taken to generate the summary.
```
Summary:

    Blockchain technology is a decentralized digital ledger that records transactions securely across a network of computers.
    Unlike traditional databases controlled by one authority, blockchain distributes identical copies of data to many nodes, reducing the risk of failure or manipulation.
    Each transaction is stored in a “block” and linked with others using cryptography, making the chain transparent, secure, and nearly impossible to alter.
    Transactions are verified through consensus methods like Proof of Work or Proof of Stake. While first used for cryptocurrencies such as Bitcoin, blockchain now benefits industries like finance, supply chain, healthcare, and even voting systems.
    It also enables “smart contracts,” which automatically execute coded agreements. Despite its promise, blockchain faces challenges in scalability, regulation, and energy use. Still, it is seen as a key technology for the digital future.
```

6. **Evaluation Criteria**
   Evaluate each generated summary using the following:

   * **Accuracy**: Does the summary correctly capture the main points of the article?
   * **Coherence**: Is the summary logically structured and easy to follow?
   * **Simplicity**: Is the language accessible for undergraduate students?
   * **Speed**: How fast is the response?
   * **User Experience**: Was the interface intuitive, and was the output easy to copy/save?

7. **Scoring & Analysis**

   * Assign scores (1 to 5) for each criterion across all combinations.
   * Tabulate results for comparison.
   * Identify the best-performing strategy-platform combination.

---

## Result

| Platform | Prompt Type      | Accuracy | Coherence | Simplicity | Speed | UX | Total (/25) |
| -------- | ---------------- | -------- | --------- | ---------- | ----- | -- | ----------- |
| ChatGPT  | Zero-shot        | 4        | 4         | 4          | 5     | 5  | 22          |
| ChatGPT  | Few-shot         | 5        | 5         | 5          | 4     | 5  | 24          |
| ChatGPT  | Chain-of-Thought | 5        | 5         | 4          | 3     | 5  | 22          |
| ChatGPT  | Role-based       | 5        | 5         | 5          | 4     | 5  | 24          |
| Gemini   | Zero-shot        | 3        | 3         | 3          | 5     | 4  | 18          |
| Gemini   | Few-shot         | 4        | 4         | 4          | 4     | 4  | 20          |
| Claude   | Chain-of-Thought | 5        | 5         | 5          | 4     | 4  | 23          |
| Claude   | Role-based       | 5        | 5         | 5          | 4     | 5  | 24          |
| Copilot  | Zero-shot        | 3        | 3         | 3          | 5     | 4  | 18          |
| Copilot  | Few-shot         | 4        | 4         | 4          | 4     | 4  | 20          |

### PICTORIAL GRAPH
<img width="2400" height="1600" alt="image" src="https://github.com/user-attachments/assets/223662a6-cf71-409a-b2c1-8e723b13dfde" />



> **Best Performing Combination:**
> **Claude + Role-based Prompting** and **ChatGPT + Few-shot Prompting** both scored **24/25**, showing high effectiveness in summarizing complex content in a simple and structured way for undergraduates.




