# JTAG/SWD Interface

CWE-1191

Risk: Information Exposure

## Description

JTAG and Serial Wire Debug (SWD) interfaces allow access to firmware and debugging capabilities during development. These must not be accessible in production, and the security fuse should be blown. The interface should be identified on the hardware of a device and verified to be inaccessible before deployment.

_Note: Some devices do not have header pins on the board, but access to the pins still allows access to the interface and is not a secure implementation._

## Tools

* JTAGulator
* Attify Badge
* BusPirate
* TIAO Universal Multi-Protocol Analyzer (TUMPA)

## Test

1. Identify the JTAG and/or CWD ports.
2. Usually the exposed pins will be in a group. Check if the pin interfaces for JTAG (TMI, TCK, TDI, TDO) or SWD (SWDIO, SWCLK) can be identified using a tool or via board/chip documentation.
3. Connect to the pin interfaces to verify that no interface is available for firmware upload or download.

## Results

A device will fail this test if the pins are exposed for connection and security fuse has not been blown, or any actions to the firmware including modification and execution can be done.

## Impact


