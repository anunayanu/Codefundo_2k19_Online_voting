# Codefundo_2k19_Online_voting
An online  voting system project deployed on Microsoft Azure blockchain for CodeFundo++ 2k19

## Secure and Decentralized voting System

## Problems faced by existing voting systems

- Long Queue on poling booths.
- Delay between end of voting and results.
- Somepeople want to vote but they don't want to go outside.
- Lack of transparency
- Duplicate Votes.

## What and how our application solve this

### Two seperate datasets
  - One  standard relational database of all valid voters, for fast querying.
  - The other will be the the blockchain of all the cast votes, for immutability and verifiablity.
  
### Multi-party encryption to enable vote transparency.  
  
## Working  

- Each voter ID is randomly assigned a SHA256 token which is linked to his/her Aadhaar ID/Voter-ID. 

- Voters will be required to login using their Aadhar ID/Voter-ID and fingerprint (for biometric verification).The token generated on successful login can be used to vote and is registered on the blockchain.The vote is encrypted such that only the voter and the election authority's combined secret id can access it.

- anonymized voting with metadata enables analytics. Metadata is stored as json so any no-sql DBMS can be used to run rich queries and generate insights.

- Once the election ends and the shared secret is put together, all the votes can be decrypted for rapid counting.

- Every voter will be registerd for a crypto wallet.

- Using Go-Etherium permissioned Proof of Authority(POA) blockchain.

- Hashed details like voter ID, time, Vote , IP address and location are sent through the nodes(blocks).

## Technologies Used:
- Azure Blockchain Services as cloud computing Service

-	GitHub for version control

-	Go-Etherium(Geth) blockchain framework

-	Azure SQL database

- SHA1 algorithm

- HTML, CSS, Javascript for frontend


