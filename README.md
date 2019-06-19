# POC 01
It is verifying how we can build the contract for some idea. 

e.g. create a contract via a contract.

---

## Features
There are two contracts in the sol file.
It seems some simple interaction, but can help us to understand how we can implement and what service we might need.
### OtoCorpLLC
- **constructor**: Sets `msg.sender` as the manager of the contract.
- **getBalance**: Gets the balance of the contract.
- **withdraw**: Transfers the balance to the manager. (Only manager can do)
- **createSeries**: Pay 0.1 ETH to create a Series(Contract) and set its name, symbol, total shares. Records its address to series array and a hashtable to the creator(`msg.sender`).
- **getMySeries**: Get an address array of all my series.

### Series
- **constructor**: Sets some attribute to initialize a Series.
- **getCreator**: Get creator address.
- **setMember**: Set a member.