# Sandbox lesson 1: The Direct Link (Peer-to-Peer)

_Level: Beginner — BuildTheNet 3D Sandbox_

**Status: Verified.** Completed on 2026-11-23; every requirement was machine-checked against the network built in BuildTheNet and passed.

Snapshot taken 2026-11-23. Built in a simulation — no physical or production equipment was involved.

## Scenario

Welcome to Cisco Simulation! Direct device-to-device communication between similar devices traditionally requires a crossover cable. Connect two PCs and establish ICMP communication.

## Objective

Place 2 PCs on canvas. Connect them with a Crossover cable. Configure IP addresses in 192.168.1.0/24 (e.g. 192.168.1.10 and 192.168.1.11). Ensure both interfaces are UP and ping between them.

## Checks

| # | Check | Status | Checked by |
|---|---|---|---|
| 1 | Place 2 PCs on canvas. Connect them with a Crossover cable. Configure IP addresses in 192.168.1.0/24 (e.g. 192.168.1.10 and 192.168.1.11). Ensure both interfaces are UP and ping between them. | Passed | Sandbox check |

## Result

The lesson's check passed on this snapshot:

> Ping successful! Direct link communication confirmed.

## What I did

Built from an empty canvas: 2 devices and 1 cable.

- PC-1 (PC): 192.168.1.11 255.255.255.0, gateway 192.168.1.1
- PC-2 (PC): 192.168.1.10 255.255.255.0, gateway 192.168.1.1

- Cabled PC-1 Eth0 to PC-2 Eth0

## Topology

![Topology diagram](topology.svg)

## Addressing

| Device | Interface | Address | Mask | Mode | Gateway |
|---|---|---|---|---|---|
| PC-1 | Eth0 | 192.168.1.11/24 | 255.255.255.0 | VLAN 1 | 192.168.1.1 |
| PC-2 | Eth0 | 192.168.1.10/24 | 255.255.255.0 | VLAN 1 | 192.168.1.1 |

---

Built on [BuildTheNet](https://www.buildthenet.io/sandbox)
