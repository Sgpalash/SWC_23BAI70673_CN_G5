# 1) IP ADDRESS
An **IP (Internet Protocol) Address** is a unique logical address assigned to every device connected to a network. It helps identify the source and destination devices for communication.

### TYPES OF IP ADDRESS
| IPv4 | 32-bit address (4 Octets) | Example: 192.168.1.10 |
|-|-|-|
| IPv6 | 128-bit address | Example: 2001:db8::1 |

### IPv4 FORMAT
```
192 . 168 . 10 . 5
 ↑      ↑      ↑     ↑
Octet  Octet  Octet Octet
```

- Consists of **32 bits**
- Divided into **4 octets**
- Each octet contains **8 bits**
- Value of each octet ranges from **0 to 255**

### BINARY REPRESENTATION

|Decimal|Binary|
|-|-|
|0|00000000|
|1|00000001|
|10|00001010|
|100|01100100|
|192|11000000|
|255|11111111|

### NETWORK ID & HOST ID

The IP address is divided into two parts:

- **Network ID** → Identifies the network.
- **Host ID** → Identifies the device inside that network.

Example:

```
IP Address : 192.168.10.25
Subnet Mask: 255.255.255.0

Network ID = 192.168.10.0
Host ID    = 25
```

<br><br>

# 2) IP ADDRESS CLASSES

IPv4 addresses are divided into **5 classes**.

|Class|First Octet Range|Default Subnet Mask|Usage|
|-|-|-|-|
|A|1 - 126|255.0.0.0|Large Networks|
|B|128 - 191|255.255.0.0|Medium Networks|
|C|192 - 223|255.255.255.0|Small Networks|
|D|224 - 239|N/A|Multicasting|
|E|240 - 255|N/A|Research & Experimental|

### CLASS IDENTIFICATION

|Class|Starts With Binary|
|-|-|
|A|0xxxxxxx|
|B|10xxxxxx|
|C|110xxxxx|
|D|1110xxxx|
|E|1111xxxx|

### SPECIAL IP ADDRESSES

|127.x.x.x|Loopback Address|
|-|-|
|0.0.0.0|Default Network|
|255.255.255.255|Broadcast Address|

<br><br>

# 3) PUBLIC vs PRIVATE IP ADDRESS

### PUBLIC IP
- Assigned by ISP.
- Accessible over the Internet.
- Globally unique.

### PRIVATE IP
- Used inside Local Area Networks.
- Cannot be accessed directly from the Internet.

|Class|Private Range|
|-|-|
|A|10.0.0.0 – 10.255.255.255|
|B|172.16.0.0 – 172.31.255.255|
|C|192.168.0.0 – 192.168.255.255|

<br><br>

# 4) SUBNET MASK

A **Subnet Mask** is a 32-bit number that separates the **Network ID** from the **Host ID**.

Example:

```
IP Address : 192.168.1.25

Subnet Mask:
255.255.255.0

Binary:
11111111.11111111.11111111.00000000
```

- **1 → Network Portion**
- **0 → Host Portion**

### COMMON SUBNET MASKS

|CIDR|Subnet Mask|
|-|-|
|/8|255.0.0.0|
|/16|255.255.0.0|
|/24|255.255.255.0|
|/25|255.255.255.128|
|/26|255.255.255.192|
|/27|255.255.255.224|
|/28|255.255.255.240|
|/29|255.255.255.248|
|/30|255.255.255.252|

<br><br>

# 5) SUBNETTING

Subnetting is the process of dividing one large network into multiple smaller networks (subnets).

### ADVANTAGES

- Better network management
- Reduced Broadcast Traffic
- Improved Security
- Efficient IP Address Utilization
- Better Performance

### FORMULAS

Number of Subnets

```
2ⁿ
```

where **n = Borrowed Host Bits**

Number of Hosts

```
2ʰ − 2
```

where **h = Remaining Host Bits**

(-2 because Network Address and Broadcast Address cannot be assigned to hosts.)

<br><br>

# 6) CIDR (Classless Inter-Domain Routing)

CIDR uses **prefix notation** instead of default classes.

Example:

```
192.168.1.0/24
```

Here,

- /24 → 24 Network Bits
- Remaining 8 bits → Host Bits

### EXAMPLES

|CIDR|Hosts|
|-|-:|
|/24|254|
|/25|126|
|/26|62|
|/27|30|
|/28|14|
|/29|6|
|/30|2|

<br><br>

# 7) HOW TO FIND NETWORK & BROADCAST ADDRESS

### Example

```
IP Address = 192.168.1.130
Subnet Mask = 255.255.255.192 (/26)
```

### Step 1

Block Size

```
256 - 192 = 64
```

Subnets

```
0
64
128
192
```

Since **130** lies between **128–191**

### RESULT

|Network Address|192.168.1.128|
|-|-|
|First Host|192.168.1.129|
|Last Host|192.168.1.190|
|Broadcast Address|192.168.1.191|

<br><br>

# 8) QUICK SUBNETTING TABLE

|CIDR|Subnet Mask|Block Size|Hosts|
|-|-|-|-:|
|/24|255.255.255.0|256|254|
|/25|255.255.255.128|128|126|
|/26|255.255.255.192|64|62|
|/27|255.255.255.224|32|30|
|/28|255.255.255.240|16|14|
|/29|255.255.255.248|8|6|
|/30|255.255.255.252|4|2|

<br><br>

# 9) SUBNETTING STEPS

1. Write the IP Address.
2. Write the Subnet Mask.
3. Find the Block Size.
4. Identify the Network Range.
5. Find the Network Address.
6. Find the Broadcast Address.
7. Find the First Host.
8. Find the Last Host.

<br><br>

# ABBREVIATIONS

|IP|Internet Protocol|
|-|-|
|IPv4|Internet Protocol Version 4|
|IPv6|Internet Protocol Version 6|
|CIDR|Classless Inter-Domain Routing|
|ISP|Internet Service Provider|
|LAN|Local Area Network|
|WAN|Wide Area Network|
|MAC|Media Access Control|
|ID|Identifier|
|NID|Network Identifier|
|HID|Host Identifier|
|PDU|Protocol Data Unit|
|DNS|Domain Name System|
|DHCP|Dynamic Host Configuration Protocol|
|NAT|Network Address Translation|
|FLSM|Fixed Length Subnet Mask|
|VLSM|Variable Length Subnet Mask|
