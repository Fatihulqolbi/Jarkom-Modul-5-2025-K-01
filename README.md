# Jarkom-Modul-5-2025-K-01

| Nama                                  | NRP        |
| ------------------------------------- | ---------- | 
| Muhammad Fatihul Qolbi Ash Shiddiqi   | 5027241023 | 
| Hansen Chang                          | 5027241028 |

## Topologi 
<img width="1505" height="768" alt="Screenshot 2025-11-29 160413" src="https://github.com/user-attachments/assets/d392d6c5-68c3-4077-bd8f-f933b7281c50" />

## Topologi VLSM
<img width="2332" height="1186" alt="Modul 5 Jarkom drawio" src="https://github.com/user-attachments/assets/93799264-a19d-4565-bfab-b255594ee6a5" />

## Tabel Rute

| Nama Subnet | Rute                                                | Jumlah IP | Netmask |
|-------------|------------------------------------------------------|-----------|---------|
| A1          | Moria → Switch1 → IronHills                          | 2         | /30     |
| A2          | Moria → Wonderland                                   | 2         | /30     |
| A3          | Wonderland → Durin                                   | 51        | /26     |
| A4          | Wonderland → Switch2 → Khamul                        | 6         | /29     |
| A5          | Osgiliath → Moria                                    | 2         | /30     |
| A6          | Osgiliath → Rivendell                                | 2         | /30     |
| A7          | Rivendell → Switch3 → Vilya → Narya                  | 2         | /30     |
| A8          | Osgiliath → Minastir                                 | 3         | /29     |
| A9          | Minastir → Pelargir                                  | 2         | /30     |
| A10         | Minastir → Switch4 → Isildur → Elendil               | 231       | /24     |
| A11         | Pelargir → Palantir                                  | 2         | /30     |
| A12         | Pelargir → AnduinBanks                               | 2         | /30     |
| A13         | AnduinBanks → Switch5 → Gilgalad → Cirdan            | 121       | /25     |
| **Total**   |                                                      | **428**   | **/23** |

<img width="824" height="371" alt="Screenshot 2025-11-29 170115" src="https://github.com/user-attachments/assets/d6c9148d-a633-47da-8c09-dc4392b6d005" />

## Tree 

<img width="1055" height="547" alt="image" src="https://github.com/user-attachments/assets/4a052fb3-e681-4aa1-b165-7251de492975" />

## Pembagian IP

## Tabel 3 – Hasil Perhitungan VLSM (A1–A13)

## Tabel Subnet

| Subnet | Network ID   | Netmask         | Broadcast     | Range IP                         |
|--------|--------------|-----------------|---------------|----------------------------------|
| A10    | 10.64.0.0    | 255.255.255.0   | 10.64.0.255   | 10.64.0.1 – 10.64.0.254           |
| A13    | 10.64.1.0    | 255.255.255.128 | 10.64.1.127   | 10.64.1.1 – 10.64.1.126           |
| A3     | 10.64.1.128  | 255.255.255.192 | 10.64.1.191   | 10.64.1.129 – 10.64.1.190         |
| A4     | 10.64.1.192  | 255.255.255.248 | 10.64.1.199   | 10.64.1.193 – 10.64.1.198         |
| A8     | 10.64.1.200  | 255.255.255.248 | 10.64.1.207   | 10.64.1.201 – 10.64.1.206         |
| A1     | 10.64.1.208  | 255.255.255.252 | 10.64.1.211   | 10.64.1.209 – 10.64.1.210         |
| A2     | 10.64.1.212  | 255.255.255.252 | 10.64.1.215   | 10.64.1.213 – 10.64.1.214         |
| A5     | 10.64.1.216  | 255.255.255.252 | 10.64.1.219   | 10.64.1.217 – 10.64.1.218         |
| A6     | 10.64.1.220  | 255.255.255.252 | 10.64.1.223   | 10.64.1.221 – 10.64.1.222         |
| A7     | 10.64.1.224  | 255.255.255.252 | 10.64.1.227   | 10.64.1.225 – 10.64.1.226         |
| A9     | 10.64.1.228  | 255.255.255.252 | 10.64.1.231   | 10.64.1.229 – 10.64.1.230         |
| A11    | 10.64.1.232  | 255.255.255.252 | 10.64.1.235   | 10.64.1.233 – 10.64.1.234         |
| A12    | 10.64.1.236  | 255.255.255.252 | 10.64.1.239   | 10.64.1.237 – 10.64.1.238         |

## LEBIH LENGKAPNYA

| Name | Hosts Needed | Hosts Available | Unused Hosts | Network Address | Slash | Mask             | Usable Range                   | Broadcast   |
|------|--------------|-----------------|-------------|-----------------|-------|------------------|--------------------------------|------------|
| A10  | 231          | 254             | 23          | 10.64.0.0       | /24   | 255.255.255.0    | 10.64.0.1 – 10.64.0.254        | 10.64.0.255 |
| A13  | 121          | 126             | 5           | 10.64.1.0       | /25   | 255.255.255.128  | 10.64.1.1 – 10.64.1.126        | 10.64.1.127 |
| A3   | 51           | 62              | 11          | 10.64.1.128     | /26   | 255.255.255.192  | 10.64.1.129 – 10.64.1.190      | 10.64.1.191 |
| A4   | 6            | 6               | 0           | 10.64.1.192     | /29   | 255.255.255.248  | 10.64.1.193 – 10.64.1.198      | 10.64.1.199 |
| A8   | 3            | 6               | 3           | 10.64.1.200     | /29   | 255.255.255.248  | 10.64.1.201 – 10.64.1.206      | 10.64.1.207 |
| A1   | 2            | 2               | 0           | 10.64.1.208     | /30   | 255.255.255.252  | 10.64.1.209 – 10.64.1.210      | 10.64.1.211 |
| A2   | 2            | 2               | 0           | 10.64.1.212     | /30   | 255.255.255.252  | 10.64.1.213 – 10.64.1.214      | 10.64.1.215 |
| A5   | 2            | 2               | 0           | 10.64.1.216     | /30   | 255.255.255.252  | 10.64.1.217 – 10.64.1.218      | 10.64.1.219 |
| A6   | 2            | 2               | 0           | 10.64.1.220     | /30   | 255.255.255.252  | 10.64.1.221 – 10.64.1.222      | 10.64.1.223 |
| A7   | 2            | 2               | 0           | 10.64.1.224     | /30   | 255.255.255.252  | 10.64.1.225 – 10.64.1.226      | 10.64.1.227 |
| A9   | 2            | 2               | 0           | 10.64.1.228     | /30   | 255.255.255.252  | 10.64.1.229 – 10.64.1.230      | 10.64.1.231 |
| A11  | 2            | 2               | 0           | 10.64.1.232     | /30   | 255.255.255.252  | 10.64.1.233 – 10.64.1.234      | 10.64.1.235 |
| A12  | 2            | 2               | 0           | 10.64.1.236     | /30   | 255.255.255.252  | 10.64.1.237 – 10.64.1.238      | 10.64.1.239 |

## Config Jarkom MISI 1

### Osgiliath
```
nano /etc/rc.local

#!/bin/sh

# Bersihkan dulu biar gak dobel
ip addr flush dev eth1
ip addr flush dev eth2
ip addr flush dev eth3

# A5: ke Moria
ip addr add 10.64.1.218/30 dev eth1
# A6: ke Rivendell
ip addr add 10.64.1.221/30 dev eth2
# A8: ke Minastir
ip addr add 10.64.1.201/29 dev eth3

ip link set eth1 up
ip link set eth2 up
ip link set eth3 up

echo 1 > /proc/sys/net/ipv4/ip_forward

# ====== ROUTING KIRI (menuju IronHills, Durin, Khamul) ======
# A1 Moria–IronHills
ip route add 10.64.1.208/30 via 10.64.1.217
# A3 Durin
ip route add 10.64.1.128/26 via 10.64.1.217
# A4 Khamul
ip route add 10.64.1.192/29 via 10.64.1.217
# A2 Moria–Winderland
ip route add 10.64.1.212/30 via 10.64.1.217

# ====== ROUTING KANAN (menuju Elendil, Isildur, Palantir, Gilgalad, Cirdan) ======
# Semua via Minastir (10.64.1.202)
ip route add 10.64.0.0/24   via 10.64.1.202   # Elendil & Isildur (A10)
ip route add 10.64.1.228/30 via 10.64.1.202   # Minastir–Pelargir (A9)
ip route add 10.64.1.232/30 via 10.64.1.202   # Pelargir–Palantir (A11)
ip route add 10.64.1.236/30 via 10.64.1.202   # Pelargir–AnduinBanks (A12)
ip route add 10.64.1.0/25   via 10.64.1.202   # Gilgalad & Cirdan (A13)

exit 0

chmod +x /etc/rc.local
/etc/rc.local
echo "/etc/rc.local" >> /etc/profile
```

### Moria
```
nano /etc/rc.local

#!/bin/sh

ip addr flush dev eth0
ip addr flush dev eth1
ip addr flush dev eth2

# A5 ke Osgiliath
ip addr add 10.64.1.217/30 dev eth0
# A1 ke IronHills
ip addr add 10.64.1.209/30 dev eth1
# A2 ke Winderland
ip addr add 10.64.1.213/30 dev eth2

ip link set eth0 up
ip link set eth1 up
ip link set eth2 up

echo 1 > /proc/sys/net/ipv4/ip_forward

# Default ke Osgiliath
ip route add default via 10.64.1.218

# LAN di belakang Winderland
ip route add 10.64.1.128/26 via 10.64.1.214   # Durin
ip route add 10.64.1.192/29 via 10.64.1.214   # Khamul

exit 0


chmod +x /etc/rc.local
/etc/rc.local

```

### Winderland
```
#!/bin/sh

ip addr flush dev eth0
ip addr flush dev eth1
ip addr flush dev eth2

# A2: ke Moria
ip addr add 10.64.1.214/30 dev eth0
# A3: Durin LAN
ip addr add 10.64.1.129/26 dev eth1
# A4: Khamul LAN
ip addr add 10.64.1.193/29 dev eth2

ip link set eth0 up
ip link set eth1 up
ip link set eth2 up

echo 1 > /proc/sys/net/ipv4/ip_forward

ip route add default via 10.64.1.213

exit 0

```

### Durim
```
#!/bin/sh

ip addr flush dev eth0
ip addr add 10.64.1.130/26 dev eth0
ip link set eth0 up

ip route add default via 10.64.1.129   # Winderland

exit 0
```

### Khamul
```
#!/bin/sh

ip addr flush dev eth0
ip addr add 10.64.1.194/29 dev eth0
ip link set eth0 up

ip route add default via 10.64.1.193   # Winderland

exit 0
```

### IronHills
```
#!/bin/sh

ip addr flush dev eth0

# A1: Moria–IronHills
ip addr add 10.64.1.210/30 dev eth0
ip link set eth0 up

ip route add default via 10.64.1.209   # Moria

exit 0
```

### Rivendell
```
#!/bin/sh

ip addr flush dev eth0

# A6: ke Osgiliath
ip addr add 10.64.1.222/30 dev eth0
ip link set eth0 up

echo 1 > /proc/sys/net/ipv4/ip_forward

ip route add default via 10.64.1.221

exit 0
```

### Vilya
```
#!/bin/sh

ip addr flush dev eth0
ip addr add 10.64.1.226/29 dev eth0    # kamu boleh pakai /29 di sini
ip link set eth0 up

ip route add default via 10.64.1.225   # Rivendell

exit 0
```

### Narya
```
#!/bin/sh

ip addr flush dev eth0
ip addr add 10.64.1.227/29 dev eth0
ip link set eth0 up

ip route add default via 10.64.1.225   # Rivendell

exit 0
```

### Minastir
```
#!/bin/sh

ip addr flush dev eth0
ip addr flush dev eth1
ip addr flush dev eth2

# A8: ke Osgiliath
ip addr add 10.64.1.202/29 dev eth0
# A9: ke Pelargir
ip addr add 10.64.1.229/30 dev eth1
# A10: LAN Elendil & Isildur
ip addr add 10.64.0.1/24 dev eth2

ip link set eth0 up
ip link set eth1 up
ip link set eth2 up

echo 1 > /proc/sys/net/ipv4/ip_forward

ip route add default via 10.64.1.201   # Osgiliath

# Jaringan di belakang Pelargir
ip route add 10.64.1.232/30 via 10.64.1.230   # Palantir
ip route add 10.64.1.236/30 via 10.64.1.230   # AnduinBanks
ip route add 10.64.1.0/25  via 10.64.1.230   # Gilgalad & Cirdan

exit 0
```

### Elendil
```
#!/bin/sh

ip addr flush dev eth0
ip addr add 10.64.0.2/24 dev eth0
ip link set eth0 up

ip route add default via 10.64.0.1   # Minastir

exit 0
```

### Isildur
```
#!/bin/sh

ip addr flush dev eth0
ip addr add 10.64.0.3/24 dev eth0
ip link set eth0 up

ip route add default via 10.64.0.1

exit 0

```

### Pelargir
```
#!/bin/sh

ip addr flush dev eth0
ip addr flush dev eth1
ip addr flush dev eth2

# A9: ke Minastir
ip addr add 10.64.1.230/30 dev eth0
# A12: ke AnduinBanks
ip addr add 10.64.1.237/30 dev eth1
# A11: ke Palantir
ip addr add 10.64.1.233/30 dev eth2

ip link set eth0 up
ip link set eth1 up
ip link set eth2 up

echo 1 > /proc/sys/net/ipv4/ip_forward

ip route add default via 10.64.1.229

# LAN Gilgalad & Cirdan via AnduinBanks
ip route add 10.64.1.0/25 via 10.64.1.238

exit 0

```

### Palantir
```
#!/bin/sh

ip addr flush dev eth0

# A11: Pelargir–Palantir
ip addr add 10.64.1.234/30 dev eth0
ip link set eth0 up

ip route add default via 10.64.1.233

exit 0

```

### AnduinBanks
```
#!/bin/sh

ip addr flush dev eth0
ip addr flush dev eth1

# A12: Pelargir–AnduinBanks
ip addr add 10.64.1.238/30 dev eth0
# A13: LAN elf
ip addr add 10.64.1.1/25 dev eth1

ip link set eth0 up
ip link set eth1 up

echo 1 > /proc/sys/net/ipv4/ip_forward

ip route add default via 10.64.1.237   # Pelargir

exit 0
```

### Gilgalad
```
#!/bin/sh

ip addr flush dev eth0
ip addr add 10.64.1.10/25 dev eth0
ip link set eth0 up

ip route add default via 10.64.1.1   # AnduinBanks

exit 0
```

### Cirdan
```
#!/bin/sh

ip addr flush dev eth0
ip addr add 10.64.1.20/25 dev eth0
ip link set eth0 up

ip route add default via 10.64.1.1

exit 0
```

### Uji Coba ( Ping antar Node )
```
Di IronHills :

ping 10.64.1.209    # Moria
ping 10.64.1.218    # Osgiliath
ping 10.64.1.202    # Minastir
ping 10.64.1.230    # Pelargir
ping 10.64.1.238    # AnduinBanks
ping 10.64.1.20     # Cirdan
```

## MISI 2 No 1

### Osgiliath
```
nano /etc/rc.local

#!/bin/sh

#############################################
# OSGILIATH – ROUTER PUSAT + GATEWAY INTERNET
#############################################

# ===========================================
# 1. Aktifkan IP FORWARDING
# ===========================================
echo 1 > /proc/sys/net/ipv4/ip_forward



# ===========================================
# 2. IP ADDRESS INTERFACE INTERNAL (10.64.x.x)
# ===========================================

# Reset interface internal
ip addr flush dev eth1 2>/dev/null
ip addr flush dev eth2 2>/dev/null
ip addr flush dev eth3 2>/dev/null

# A5 – Osgiliath → Moria
ip addr add 10.64.1.218/30 dev eth1

# A6 – Osgiliath → Rivendell
ip addr add 10.64.1.221/30 dev eth2

# A8 – Osgiliath → Minastir
ip addr add 10.64.1.201/29 dev eth3

ip link set eth1 up
ip link set eth2 up
ip link set eth3 up



# ===========================================
# 3. ROUTING INTERNAL A1–A13
# ===========================================

# KIRI – menuju Moria → Winderland → Durin/Khamul/IronHills
ip route add 10.64.1.208/30 via 10.64.1.217  # A1 IronHills
ip route add 10.64.1.128/26 via 10.64.1.217  # A3 Durin
ip route add 10.64.1.192/29 via 10.64.1.217  # A4 Khamul
ip route add 10.64.1.212/30 via 10.64.1.217  # A2 Winderland

# KANAN – via Minastir
ip route add 10.64.0.0/24   via 10.64.1.202  # A10 Elendil & Isildur
ip route add 10.64.1.228/30 via 10.64.1.202  # A9 Pelargir
ip route add 10.64.1.232/30 via 10.64.1.202  # A11 Palantir
ip route add 10.64.1.236/30 via 10.64.1.202  # A12 AnduinBanks
ip route add 10.64.1.0/25   via 10.64.1.202  # A13 Gilgalad & Cirdan



# ===========================================
# 4. KONFIGURASI INTERNET (eth0)
# ===========================================

# Untuk GNS3 NAT, gunakan network default:
# 192.168.122.0/24 (virbr0)
# Ganti IP jika NAT kamu beda

ip addr flush dev eth0 2>/dev/null
ip addr add 192.168.122.100/24 dev eth0
ip link set eth0 up

ip route del default 2>/dev/null
ip route add default via 192.168.122.1

# DNS untuk resolusi domain
echo "nameserver 8.8.8.8"  > /etc/resolv.conf
echo "nameserver 8.8.4.4" >> /etc/resolv.conf



# ===========================================
# 5. FIREWALL NAT TANPA MASQUERADE (SNAT)
# ===========================================

# Bersihkan aturan lama
iptables -t nat -F
iptables -F FORWARD

# NAT: GUNAKAN IP eth0
iptables -t nat -A POSTROUTING -o eth0 -j SNAT --to-source 192.168.122.100



# ===========================================
# 6. FORWARD LAN <-> INTERNET
# ===========================================

iptables -A FORWARD -i eth1 -o eth0 -j ACCEPT
iptables -A FORWARD -i eth2 -o eth0 -j ACCEPT
iptables -A FORWARD -i eth3 -o eth0 -j ACCEPT

iptables -A FORWARD -i eth0 -o eth1 -j ACCEPT
iptables -A FORWARD -i eth0 -o eth2 -j ACCEPT
iptables -A FORWARD -i eth0 -o eth3 -j ACCEPT



exit 0

```

### Tambakan ke setiap node - Agar Bisa Ping google.com
```
nano /etc/rc.local

echo "nameserver 8.8.8.8"  > /etc/resolv.conf
echo "nameserver 8.8.4.4" >> /etc/resolv.conf
```
