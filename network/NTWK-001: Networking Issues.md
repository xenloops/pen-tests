# Networking Issues

CWE-923

Risk: Information Exposure

## Description

When a system can be networked, its attack surface increases dramatically. To help reduce these risks, certain basic networking techniques must be supported by the system (such as the ability to reside on a segmented network). This test examines common networking flaws that may increase not only the attack surface of the system but also may place the underlying environment at risk.

## Tools

* Wireshark
* Manual

## Test

1. Confirm that the system can be segmented on a network so as to allow physical and logical isolation of the system.
2. Confirm that the system is capable of carrying out its network functions without requiring networks that would otherwise be outside the scope of the system.

## Results

1. If the device does not allow networking to facilitate segmentation, this test fails.
2. If the system requires access to networks beyond the boundaries of the system, this test fails

## Impact
