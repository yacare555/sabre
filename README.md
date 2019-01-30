# Sabre

Minimum viable [MythX](https://mythx.io) client. Compiles and analyzes a single Solidity smart contract.

## Usage

1. Use Metamask to sign up for an account on the [MythX website](https://mythx.io) and set your API password.

2. Get the code:

```
$ git clone https://github.com/b-mueller/sabre/
$ cd sabre
```

3. Set up your environment. Use the Ethereum address you signed up with as the username.

```
export MYTHX_API_URL=https://api.mythx.io
export MYTHX_ETH_ADDRESS=0x(...)
export MYTHX_PASSWORD=password
```

4. Run an analysis:

```
$ node sabre.js mycontract.sol 

__mycontract.sol __
3     Low     State Variable Default Visibility    https://smartcontractsecurity.github.io/SWC-registry/docs/SWC-108
5     Low     Function Default Visibility          https://smartcontractsecurity.github.io/SWC-registry/docs/SWC-100
14    High    Reentrancy                           https://smartcontractsecurity.github.io/SWC-registry/docs/SWC-107
```

## Usage

See also:

- [Armlet client library](https://github.com/ConsenSys/armlet)
- [MythX documentation](https://docs.mythx.io/en/latest/)
