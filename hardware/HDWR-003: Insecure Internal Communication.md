# Insecure Internal Communication Bus and Protocol

Risk: Injection

## Description



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
