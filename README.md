# WSYS
<img src="img/logo.png" width="200">

WSYS or Wrapped SYS is an [ERC-20](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-20.md) compatible wrapper contract around the Syscoin token.

On Syscoin NEVM, SYS is treated just like standard ETH is on Ethereum. This means that SYS lacks the standardized interfaces that make ERC-20 tokens so interchangeable. WSYS corrects this by issuing one ERC-20 WSYS token for each SYS deposited. Each WSYS is then redeemable for an equal amount of SYS.

## Implementation
WSYS is based on the implementation of Canonical WETH developed by the Ethereum community. Details are available [here](https://blog.0xproject.com/canonical-weth-a9aa7d0279dd) and original source code is available here: https://github.com/gnosis/canonical-weth.

The WSYS implementation only changes the underlying contract to reflect the new token name of "Wrapped SYS" and the new symbol "WSYS."

## Security
Because this contract is a fork of canonical WETH, it has the same security characteristics of the Gnosis WETH implementation. That contract has been in circulation for several years and has been thoroughly audited.

## Deployment
- NEVM: [0xd3e822f3ef011Ca5f17D82C956D952D8d7C3A1BB](https://explorer.syscoin.org/token/0xd3e822f3ef011Ca5f17D82C956D952D8d7C3A1BB)
- Tanenbaum Testnet: [0xa66b2E50c2b805F31712beA422D0D9e7D0Fd0F35](https://tanenbaum.io/address/0xa66b2E50c2b805F31712beA422D0D9e7D0Fd0F35)

