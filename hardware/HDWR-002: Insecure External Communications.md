# Insecure External Communication Bus and Protocol

Risks: Component Vulnerabilities, Information Exposure

## Description

An internal or external communication bus may be implemented on a controller or system using a variety of protocols. These physical interfaces and protocols can be susceptible to interference or leakage of sensitive information. Building automation and control protocols can be susceptible to attacks due to their insecure formats. Protocols like Niagara4, SYLK, BACNet, Nano, while unencrypted, should not allow malicious behavior to impact device performance.

Note that this test case specifically applies to buses that are external to chips. 1-wire, I2C, etc. are covered by HDWR-003: Insecure Internal Communication.

## Tools

* Attify Badge
* BusPirate
* TIAO Universal Multi-Protocol Analyzer (TUMPA)

## Test

1. Identify com ports.
2. Connect to the device under test and capture traffic coming from the device.
3. Attempt to capture cleartext information from the device.
4. Replay data, whether corrupted or modified, onto the network and check for expected behavior resulting from planned attack method.

## Results

Transmission of data over the protocol will result in a failure if it can result in behavioral changes of the device such as reinitialization or deletion, excessive privileges or improper resource allocation, or the ability to capture unencrypted sensitive information.

## Impact
