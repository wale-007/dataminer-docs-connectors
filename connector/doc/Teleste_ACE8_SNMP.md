---
uid: Connector_help_Teleste_ACE8_SNMP
---

# Teleste ACE8 SNMP

ACE8 is an intelligent node with one active output, which may be split internally in two. It offers a high output level (Umax 138 QAM/111.5 dBμV) and supports 1.2 GHz downstream and up to 204 MHz upstream frequencies.

This connector uses an SNMP connection to poll data from the ACE8 device.

## About

### Version Info

| Range              | Key Features     | Based on     | System Impact     |
|--------------------|------------------|--------------|-------------------|
| 1.0.0.x [SLC Main] | Initial version  | -            | -                 |

### Product Info

| Range     | Supported Firmware     |
|-----------|------------------------|
| 1.0.0.x   | 4.8.13                 |

### System Info

| Range   | DCF Integration | Cassandra Compliant | Linked Components | Exported Components |
|---------|-----------------|---------------------|-------------------|---------------------|
| 1.0.0.x | No              | Yes                 | -                 | -                   |

## Configuration

### Connections

#### SNMP Main Connection

This connector uses a Simple Network Management Protocol (SNMP) connection and requires the following input during element creation:

SNMP CONNECTION:

- **IP address/host**: The polling IP of the ACE8 SNMP device.
- **Device address**: Not required.

SNMP Settings:

- **Port number**: The port of the connected device, by default *161*.
- **Get community string**: The community string used when reading values from the device, by default *public*.
- **Set community string**: The community string used when setting values on the device, by default *private*.

## How to Use

The **Alarm Limits** and **Status** pages contain the most important parameters for monitoring.

The **Forward Path** and **Forward Path Settings** pages contain settings related to the **optical receivers**.

The **Return Path** and **Return Path Settings** pages contain settings related to the **return transmitters**.

The **Transponder** page contains information and settings related to the transponder.

> [!NOTE]
> **Changing the communication settings or device groups on the Transponder page** may cause the element to go into **timeout** for a couple of seconds.
