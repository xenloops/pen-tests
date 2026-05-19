# Enforce Wireless Restrictions 

CWE-284

Risk: Information Exposure

## Description

A system that makes use of wireless technologies must appropriately restrict access to the system while providing commonly-employed protection techniques. This test ensures that wireless technology is appropriately managed according to this standard.

## Tools

* Manual

## Test

Verify that any wireless functionality explicitly requires authorization to connect to the system. This may be a configuration step, pairing, or other mechanism for ensuring the device is authorized.

## Results

If the system randomly accepts unknown devices or wireless connections without authorization, the test fails.

## Impact
