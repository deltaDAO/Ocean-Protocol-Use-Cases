# Data Audit Trail
> #### A Data Exchange Logging Service on Ocean Protocol

### Abstract
An immutable data audit trail enhances transparency for and trust of participants in an open data marketplace. DLT based marketplaces like Ocean Protocol enable that all transactions are verified, stored, and audited in an ordered, transparent, and trustless way, and hence enable a Data Exchange Logging Service (DELS) by design.

## Table of Contents
- [Introduction](#introduction)
- [Ocean Protocol](#ocean-protocol)
- [Security of transactions and access logs](#security-of-transactions-and-access-logs)
- [Advantages for AI research](#advantages-for-ai-research)
- [Advantages for publishers and consumers of data assets](#advantages-for-publishers-and-consumers-of-data-assets)
- [References](#references)

## Introduction
When interacting in a data economy, the flow of data assets, access rights, and payments must be auditable to protect consumers, providers, and owners of data assets. 
**Consumers** must be sure that once they pay for a data asset, they receive access to it. Moreover, the consumers must be able to prove that they have legitimately acquired the data assets. 
**Providers and owners** must be sure that if they grant access to their data asset, they will receive a payment from the consumer. Also, owners must be sure that the purchase of and access to their asset was always legitimate and that their conditions of accessing the data set (e.g., download or compute access) were not violated.  
The auditability of a data access and monetization protocol is of vital importance and requires that all processes (regarding publication, selling, purchasing, and training) must be logged automatically and reliably. The logging functionality must be resistant to manipulation and auditable. An immutable data audit trail enhances transparency for and trust of participants in an open data marketplace.

## Ocean Protocol
Ocean Protocol and its underlying Distributed Ledger Technology (DLT) provide these requirements by design. On Ocean Market, data owners can publish data assets and offer them for download and compute access. Each data set gets tokenized. If data consumers want to download the data asset or want to purchase compute access to the data, they must obtain and spend the respective data token. Moreover, each transaction concerning a data token, which includes publishing, sale, exchange, and consumption, is logged automatically and immutable. 
So, data access is tied to data tokens which enables data auditability by design.

## Security of transactions and access logs
- **Decentralized (distributed) peer-to-peer network**
    - **Transparency**: It is transparent to every network participant which data token transactions have been made. So, the log can be audited by any participant. The asset metadata is also transparent.
    - **Availability**: Network nodes store the ledger redundantly and globally distributed.	 
- **Self-Sovereign Identity (SSI)**
    - **Control**: The market participants act on the data market using their SSI, which obsoletes a trusted authority and empowers users.	 
- **Digital signatures**
    - **Authenticity and non-repudiation (reliability)**: The authenticity of the transaction is ensured using digital signatures. After signing the transaction with the private key, the transaction issuer can no longer deny that s/he issued the transaction.	 
- **Hash functions and consensus mechanisms**
    - **Integrity**: Consensus mechanisms approve the validity of all transactions before adding them to the ledger. Once a valid transaction was added to the ledger, it is stored there permanently and irreversibly. The immutability of the ledger entries is established by cryptographic chaining (hash functions).	 
- **Tokens**
    - **Access control**: Each data service has a data token, which represents the right to access the respective service. Transfers of access rights can be managed efficiently through the transfer of data tokens.	 
- **Smart contracts**
    - **Access control**: Smart contracts assure that the owner receives the payment and prevent fraudulent transactions.
    - **Metadata integrity**: Smart contracts contain data asset metadata and are stored on-chain. Only an authorized SSI can make changes to the smart contract. So, it serves as a sole source of truth. The smart contract also defines the form of the data asset access (download or compute-access, data set or algorithm) and can ensure the integrity of data assets.	 
- **Ocean Provider**
    - **Access control**: Ocean providers ensure that authorized consumers receive the data asset (or compute access). Moreover, if the compute job was not successful, it can be repeated.
	 
## Advantages for AI research
Machine Learning (ML) scientists can benefit from an immutable data audit trail as it contributes to the Explainable AI principle. This means that data scientists can prove when and on which data set the ML model has been trained, which algorithm was used, and if the algorithm was executed successfully. So, the training becomes traceable and explainable, which increases the trust in the resulting model.

## Advantages for publishers and consumers of data assets
- Using a data audit trail, individuals and companies who provide or consume data assets on Ocean Market can track each transaction, like data access or acquisition, to approve validity. Data asset consumers can prove asset acquisition and whether they got data access after the payment. Data asset owners can prove asset ownership, provision, and whether they received the consumer’s payment. 
- Moreover, as the automated data audit trail is included by design, it obsoletes additional software for keeping track, which reduces costs, time, and effort.
- The distributed and redundant storage prevents data loss.
- Another field of application is to analyze popularity trends on consumed data assets or categories of data assets. Based on that, data can be rated, and predictions can be made. 
- An immutable and complete audit trail can also serve as a reliable source of truth for internal or external auditors.
- If a company uses personal data in the context of automated individual decision-making, including profiling (Art. 22 GDPR), it must be able to explain how the decisions were made and provide “meaningful information about the logic involved” (Art. 13(2)(f) GDPR). As discussed above, a data audit trail contributes to Explainable AI, which increases transparency and trust. As a result, companies profit by mitigating the risk of infringing the GDPR, and data subjects benefit by gaining transparent information.

## References
- Berghoff, Christian, et al. "Blockchain sicher gestalten." Konzepte, Anforderungen, Bewertungen. - Bundesamt für Sicherheit in der Informationstechnik, Bonn (2019), https://www.bsi.bund.de/SharedDocs/Downloads/DE/BSI/Krypto/Blockchain_Analyse.pdf?__blob=publicationFile&v=3
- Fridgen, Gilbert, et al. "Chancen und Herausforderungen von DLT (Blockchain) in Mobilität und Logistik." (2019) https://www.bmvi.de/SharedDocs/DE/Anlage/DG/blockchain-gutachten.pdf?__blob=publicationFile.
- “Guidance on sharing private sector data in the European data economy” / “Towards a common European data space”, https://digital-strategy.ec.europa.eu/en/news/staff-working-document-guidance-sharing-private-sector-data-european-data-economy 
- Ocean Protocol Developer Documentation, https://docs.oceanprotocol.com/
- Ocean Protocol Foundation Ltd., https://oceanprotocol.com/




