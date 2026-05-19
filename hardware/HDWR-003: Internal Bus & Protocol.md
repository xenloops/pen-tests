# Internal Communication Bus and Protocol

Risk: Injection

## Description

Semiconductor chips on the same circuitboard communicate over a bus that enables direct data transfer. A bus may operate in a manner allowing a single entity to have unidirectional control over chips on the bus. This excess control leads to the primary/secondary control topology being compromised.

Note that this specifically applies to inter-chip communication. External buses and protocols are covered by HDWR-003: Insecure External Communication.

## Tools

* BusPirate
* TIAO Universal Multi-Protocol Analyzer (TUMPA)

## Test

1. Identify 1-Wire (Dallas), UART, I2C, USART, etc. ports.
2. Connect to chip bus using exposed pins or available solder points.
3. Use BusPirate to gain control of chips or capture data transferred between chips.

## Results

A failure results from the ability to perform actions on a chip bus with elevated privileges or performing malicious behavior using only low level privileges.

## Impact
