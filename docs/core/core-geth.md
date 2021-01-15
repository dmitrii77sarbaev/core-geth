# Core-Geth Features

While CoreGeth inherits from and exposes complete feature parity with Ethereum Foundation's <sup>:registered:</sup> [ethereum/go-ethereum](https://github.com/ethereum/go-ethereum),
there are quite few things that make CoreGeth unique.

CoreGeth is sponsored by and maintained with the leadership of [ETC Labs](https://etclabs.org) with an obvious core intention of stewarding
the Ethereum Classic opinion that the reversion of transactions shouldn't be permissable. 

But the spirit of the project intends to reach beyond Ethereum and Ethereum Classic, and indeed to reimagine an EVM node software that 
approaches the EVM-based protocols as technology that can -- and should -- be generalizeable.

### EVMCv6 Support

- EVMCv6, opens possibility for use with external  EVMs (including EWASM).

### Comprehensive RPC API Service Discovery

- Comprehensive service discovery with OpenRPC at `rpc.discover`.

### Extended RPC API

- Available `trace_block` and `trace_transaction` RPC API congruent to the OpenEthereum API (including a 1000x performance improvement vs. go-ethereum's `trace_transaction` in some cases).
- Available `debug_removeTransaction` API method.

### Support for Remote Ancient Chaindata

- Remote freezer, store your `ancient` data on Amazon S3 or Storj.

### Developer Features

- A developer mode `--dev.pow` able to mock Proof-of-Work block schemas and production at representative Poisson intervals.
- Chain configuration acceptance of OpenEthereum and go-ethereum chain configuration files (and the extensibility to support _any_ chain configuration schema).
- At the code level, a 1:1 EIP/ECIP specification to implementation pattern; disentangling Ethereum Foundation :registered: hard fork opinions from code. This yields more readable code, more precise naming and conceptual representation, more testable code, and a massive step toward Ethereum as a generalizeable technology.

### (Public) Risk Management

- Public chaindata regression testing run at each push to master.

### Extended IP Support

- Myriad additional ECIP support:
    + ECBP1100 (aka MESS)
    + ECIP1099 (DAG growth limit)
    + ECIP1014 (defuse difficulty bomb), etc. :wink:
- Out-of-the-box support for Ethereum Classic, EtherSocial, Social, and MIX networks.
