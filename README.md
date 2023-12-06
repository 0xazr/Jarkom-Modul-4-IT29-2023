![screenshot-1701865335741](https://github.com/0xazr/Jarkom-Modul-4-IT29-2023/assets/54212814/b4ea0039-d822-4632-bddd-3761ac2f6933)# Jarkom Modul 4 | IT29 | 2023
- M. Azril Fathoni (5027211002)
- Ridho Husni Indrawan (5027211043)

# VLSM
![image](https://github.com/0xazr/Jarkom-Modul-4-IT29-2023/assets/54212814/012abb4d-a8d1-44fa-89ff-eb5dafeae959)
## Tree
![Jarkom_Modul4-VLSM(1)](https://github.com/0xazr/Jarkom-Modul-4-IT29-2023/assets/54212814/7e45ddca-efff-4f25-b29d-0ee4ac73b026)
## Pembagian Subnet
| Subnet | Total IP | Netmask |     Address    |  Subnet Mask    |
|--------|----------|---------|----------------|-----------------|
|  A1    | 2        |  /30    | 10.78.0.0/30   | 255.255.255.252 | 
|  A2    | 2        |  /30    | 10.78.0.4/30   | 255.255.255.252 |
|  A3    | 25       |  /27    | 10.78.0.96/27  | 255.255.255.224 |
|  A4    | 2        |  /30    | 10.78.0.8/30   | 255.255.255.252 |
|  A5    | 2        |  /30    | 10.78.0.12/30  | 255.255.255.252 |
|  A6    | 2        |  /30    | 10.78.0.16/30  | 255.255.255.252 |
|  A7    | 1023     |  /21    | 10.78.24.0/21  | 255.255.248.0   |
|  A8    | 1001     |  /22    | 10.78.8.0/22   | 255.255.252.0   |
|  A9    | 6        |  /29    | 10.78.0.48/29  | 255.255.255.248 |
|  A10   | 3        |  /29    | 10.78.0.56/29  | 255.255.255.248 |
|  A11   | 2        |  /30    | 10.78.0.20/30  | 255.255.255.252 |
|  A12   | 2        |  /30    | 10.78.0.24/30  | 255.255.255.252 |
|  A13   | 2        |  /30    | 10.78.0.28/30  | 255.255.255.252 |
|  A14   | 2        |  /30    | 10.78.0.32/30  | 255.255.255.252 |
|  A15   | 1001     |  /22    | 10.78.12.0/22  | 255.255.252.0   |
|  A16   | 255      |  /23    | 10.78.4.0/23   | 255.255.254.0   |
|  A17   | 2        |  /30    | 10.78.0.36/30  | 255.255.255.252 |
|  A18   | 31       |  /26    | 10.78.0.128/26 | 255.255.255.192 |
|  A19   | 512      |  /22    | 10.78.16.0/22  | 255.255.252.0   |
|  A20   | 127      |  /24    | 10.78.2.0/24   | 255.255.255.0   |
|  A21   | 251      |  /24    | 10.78.3.0/24   | 255.255.255.0   |
|  Total | 4255     |  /19    |      -         | 255.255.224.0   |

## Routing
### Aura
- Sisi Kanan
```
ip route 10.78.2.0 255.255.255.0 10.78.0.2
```
- Sisi Kiri
```
ip route 10.78.0.48 255.255.255.248 10.78.0.6 
ip route 10.78.0.16 255.255.255.252 10.78.0.6 
ip route 10.78.8.0 255.255.252.0 10.78.0.6 
ip route 10.78.0.12 255.255.255.252 10.78.0.6 
ip route 10.78.24.0 255.255.248.0 10.78.0.6 
ip route 10.78.0.8 255.255.255.252 10.78.0.6
ip route 10.78.0.96 255.255.255.224 10.78.0.6
```
- Sisi Bawah
```
ip route 0.0.0.0 0.0.0.0 10.78.0.21
```

### Denken
```
ip route 0.0.0.0 0.0.0.0 10.78.0.1
```

### Eisen
- Sisi Kanan
```
ip route 10.78.12.0 255.255.252.0 10.78.0.30
ip route 10.78.3.0 255.255.255.0 10.78.0.30
```
- Sisi Bawah
```
ip route 10.78.4.0 255.255.254.0 10.78.0.34
ip route 10.78.0.36 255.255.255.252 10.78.0.34
ip route 10.78.0.128 255.255.255.192 10.78.0.34
ip route 10.78.16.0 255.255.252.0 10.78.0.34
```
- Sisi Atas
```
ip route 0.0.0.0 0.0.0.0 10.78.0.22
```

### Fern
```
ip route 0.0.0.0 0.0.0.0 10.78.0.13
```

### Flamme
```
ip route 0.0.0.0 0.0.0.0 10.78.0.9
```
- Sisi Atas
```
ip route 10.78.24.0 255.255.248.0 10.78.0.14
```
- Sisi Bawah
```
ip route 10.78.0.48 255.255.255.248 10.78.0.18
```

### Frieren
- Sisi Kiri
```
ip route 10.78.0.48 255.255.255.248 10.78.0.10
ip route 10.78.0.16 255.255.255.252 10.78.0.10
ip route 10.78.8.0 255.255.252.0 10.78.0.10
ip route 10.78.0.12 255.255.255.252 10.78.0.10
ip route 10.78.24.0 255.255.248.0 10.78.0.10
```
- Sisi Kanan
```
ip route 0.0.0.0 0.0.0.0 10.78.0.5
```

### Himmel
```
ip route 0.0.0.0 0.0.0.0 10.78.0.17
```

### Lugner
```
ip route 0.0.0.0 0.0.0.0 10.78.0.29
```

### Linie
- Sisi Kiri
```
ip route 10.78.0.128 255.255.255.192 10.78.0.38
ip route 10.78.16.0 255.255.252.0 10.78.0.38
```
- Sisi Atas
```
ip route 0.0.0.0 0.0.0.0 10.78.0.33
```

### Lawine
- Sisi Kiri
```
ip route 10.78.16.0 255.255.252.0 10.78.0.130
```
- Sisi Kanan
```
ip route 0.0.0.0 0.0.0.0 10.78.0.37
```

### Heiter
```
ip route 0.0.0.0 0.0.0.0 10.78.0.129
```

# CIDR
![image](https://github.com/0xazr/Jarkom-Modul-4-IT29-2023/assets/54212814/c291115f-ca74-480c-9c13-5ab263781f5b)
## Tree
![modul4_cidr(2)](https://github.com/0xazr/Jarkom-Modul-4-IT29-2023/assets/54212814/46efb8bd-2d90-4365-827a-a6f8786c888e)

## Pembagian Subnet
| Subnet | Total IP | Netmask |     Address    |  Subnet Mask    |
|--------|----------|---------|----------------|-----------------|
|  A1    | 2        |  /30    | 10.78.3.180/30 | 255.255.255.252 | 
|  A2    | 2        |  /30    | 10.78.24.80/30 | 255.255.255.252 |
|  A3    | 25       |  /27    | 10.78.24.96/27 | 255.255.255.224 |
|  A4    | 2        |  /30    | 10.78.24.84/30 | 255.255.255.252 |
|  A5    | 2        |  /30    | 10.78.24.76/30 | 255.255.255.252 |
|  A6    | 2        |  /30    | 10.78.24.72/30 | 255.255.255.252 |
|  A7    | 1023     |  /21    | 10.78.16.0/21  | 255.255.248.0   |
|  A8    | 1001     |  /22    | 10.78.28.0/22  | 255.255.252.0   |
|  A9    | 6        |  /29    | 10.78.24.88/29 | 255.255.255.248 |
|  A10   | 3        |  /29    | 10.78.3.184/29 | 255.255.255.248 |
|  A11   | 2        |  /30    | 10.78.3.176/30 | 255.255.255.252 |
|  A12   | 2        |  /30    | 10.78.3.172/30 | 255.255.255.252 |
|  A13   | 2        |  /30    | 10.78.3.168/30 | 255.255.255.252 |
|  A14   | 2        |  /30    | 10.78.3.164/30 | 255.255.255.252 |
|  A15   | 1001     |  /22    | 10.78.8.0/22   | 255.255.252.0   |
|  A16   | 255      |  /23    | 10.78.6.0/23   | 255.255.254.0   |
|  A17   | 2        |  /30    | 10.78.3.160/30 | 255.255.255.252 |
|  A18   | 31       |  /26    | 10.78.3.192/26 | 255.255.255.192 |
|  A19   | 512      |  /22    | 10.78.12.0/22  | 255.255.252.0   |
|  A20   | 127      |  /24    | 10.78.4.0/24   | 255.255.255.0   |
|  A21   | 251      |  /24    | 10.78.5.0/24   | 255.255.255.0   |
|  Total | 4255     |  /19    |      -         | 255.255.224.0   |

| B Class | Classes   | Total IP | Netmask |
|---------|-----------|----------|---------|
| B1      | A18 + A19 | 543      |  /22

| C Class | Classes   | Total IP | Netmask |
|---------|-----------|----------|---------|
| C1      | B1 + A17  | 545      |  /22
| C2      | A9 + A6   | 8        |  /28
| C3      | A7 + A5   | 1025     |  /21

| D Class | Classes   | Total IP | Netmask |
|---------|-----------|----------|---------|
| D1      | C1 + A16  | 800      |  /22
| D2      | A21 + A15 | 1252     |  /21
| D3      | C2+C3+A8  | 2034     |  /21

| E Class | Classes   | Total IP | Netmask |
|---------|-----------|----------|---------|
| E1      | D1 + A14  | 802      |  /22
| E2      | D2 + A13  | 1254     |  /21
| E3      | D3 + A4   | 2036     |  /21

| F Class | Classes       | Total IP | Netmask |
|---------|---------------|----------|---------|
| F1      |E1+E2+A12+A10  | 2061     |  /20
| F2      |  E3+A3        | 2061     |  /20

| G Class | Classes       | Total IP | Netmask |
|---------|---------------|----------|---------|
| G1      | F1+A11        | 2063     |  /20
| G2      | F2+A2         | 2063     |  /20
| G3      | A1+A20        | 129      |  /24 

| H Class | Classes       | Total IP | Netmask |
|---------|---------------|----------|---------|
| H1      | G1+G3         | 2192     |  /20
| H2      | G2+A22        | 2065     |  /20

| I Class | Classes       | Total IP | Netmask |
|---------|---------------|----------|---------|
| I1      | H1+H2         | 4257     |  /19

# Routing

### Aura
- Sisi Kanan
```
route add -net 10.78.4.0 netmask 255.255.255.0 gw 10.78.3.182
```
- Sisi Kiri
```
route add -net 10.78.24.88 netmask 255.255.255.248 gw 10.78.24.82 
route add -net 10.78.24.72 netmask 255.255.255.252 gw 10.78.24.82 
route add -net 10.78.28.0 netmask 255.255.252.0 gw 10.78.24.82 
route add -net 10.78.24.76 netmask 255.255.255.252 gw 10.78.24.82 
route add -net 10.78.16.0 netmask 255.255.248.0 gw 10.78.24.82 
route add -net 10.78.24.84 netmask 255.255.255.252 gw 10.78.24.82
route add -net 10.78.24.96 netmask 255.255.255.224 gw 10.78.24.82
```
- Sisi Bawah
```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.78.3.178
```

### Denken
```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.78.3.181
```

### Eisen
- Sisi Kanan
```
route add -net 10.78.8.0 netmask 255.255.252.0 gw 10.78.3.170
route add -net 10.78.5.0 netmask 255.255.255.0 gw 10.78.3.170
```
- Sisi Bawah
```
route add -net 10.78.6.0 netmask 255.255.254.0 gw 10.78.3.166
route add -net 10.78.3.160 netmask 255.255.255.252 gw 10.78.3.166
route add -net 10.78.3.192 netmask 255.255.255.192 gw 10.78.3.166
route add -net 10.78.12.0 netmask 255.255.252.0 gw 10.78.3.166
```
- Sisi Atas
```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.78.3.177
```

### Fern
```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.78.24.77
```

### Flamme
```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.78.24.85
route add -net 10.78.16.0 netmask 255.255.248.0 gw 10.78.24.78
route add -net 10.78.24.88 netmask 255.255.255.248 gw 10.78.24.74
```

### Frieren
```
route add -net 10.78.24.88 netmask 255.255.255.248 gw 10.78.24.86
route add -net 10.78.24.72 netmask 255.255.255.252 gw 10.78.24.86
route add -net 10.78.28.0 netmask 255.255.252.0 gw 10.78.24.86
route add -net 10.78.24.76 netmask 255.255.255.252 gw 10.78.24.86
route add -net 10.78.16.0 netmask 255.255.248.0 gw 10.78.24.86
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.78.24.81
```

### Himmel
```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.78.24.73
```

### Lugner
```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.78.3.169
```

### Linie
- Sisi Kiri
```
route add -net 10.78.3.192 netmask 255.255.255.192 gw 10.78.3.162
route add -net 10.78.12.0 netmask 255.255.252.0 gw 10.78.3.162
```
- Sisi Atas
```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.78.3.165
```

### Lawine
- Sisi Kiri
```
route add -net 10.78.12.0 netmask 255.255.252.0 gw 10.78.3.194
```
- Sisi Kanan
```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.78.3.160
```

### Heiter
```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 10.78.3.193
```
