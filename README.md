
# XELIS-PROXY (BETA v0.1.1)
![GitHub all releases](https://img.shields.io/github/downloads/XelPool/XELIS-PROXY/total) ![GitHub language](https://img.shields.io/badge/language-Go-blue)

High performance XELIS mining proxy.

Download: [releases](https://github.com/xelpool/xelis-proxy/releases)

## Usage
XELIS-PROXY is shipped with two example scripts to mine on solo node and to pool mine on [XelPool](https://xelpool.com)

## Default ports

- Stratum: `5209` (Rigel Miner)
- Getwork: `5210`
- Xatum: `5211`

## Examples

RIGEL-MINER (GPU):
```shell
./rigel -a xelishash -o stratum+tcp://localhost:5209 -u walletaddress -w my_rig 
```

## Supported Protocols
Outgoing (the proxy can connect to pools/nodes using these protocols):
- Xatum
- Getwork
Incoming (miners can connect to the proxy using these protocols):
- Xatum
- Getwork
- Stratum

## Example configuration
An example configuration file can be found in `defaultconfig.json`

## Donation
When connected to a pool, XELIS-PROXY has a donation of 0% (no fees).
When connected to a XELIS node and solo mining, XELIS-PROXY has a donation of 0.5%.