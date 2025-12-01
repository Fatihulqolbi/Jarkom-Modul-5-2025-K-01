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
# rc.local IRONHILLS - Web server

#############################################
# 1. IP ADDRESS & ROUTING
#############################################

# Bersihkan IP lama dulu supaya tidak muncul "File exists"
ip addr flush dev eth0 2>/dev/null

# A1: Moria–IronHills
ip addr add 10.64.1.210/30 dev eth0
ip link set eth0 up

# Hapus default route lama lalu set gateway ke Moria
ip route del default 2>/dev/null
ip route add default via 10.64.1.209 dev eth0

#############################################
# 2. DNS (biar apt bisa resolve)
#############################################
echo "nameserver 8.8.8.8"  > /etc/resolv.conf
echo "nameserver 8.8.4.4" >> /etc/resolv.conf

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

### Dokumentasi
<img width="678" height="875" alt="image" src="https://github.com/user-attachments/assets/21ca67d8-d99e-4429-8e4f-38e2dc601287" />


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

### Dokumentasi

<img width="910" height="457" alt="image" src="https://github.com/user-attachments/assets/2ab6c1c6-d628-4d73-8e41-40d61860dd03" />

-----------------------------------------------------------------------------------------------------------------------------------

<img width="840" height="303" alt="image" src="https://github.com/user-attachments/assets/2d4cb66c-e19a-41be-a26b-3f571ae2446d" />

## MISI 1 No 4

### Membenahi Keselahan Config

### Rivendell
```
#!/bin/sh

# ------- BERSIHKAN DULU -------
ip addr flush dev eth0
ip addr flush dev eth1

# ------- A6: Rivendell <-> Osgiliath -------
# Network: 10.64.1.220/30 → host 10.64.1.221 & 10.64.1.222
# Anggap: Osgiliath eth2 = 10.64.1.221, Rivendell eth0 = 10.64.1.222
ip addr add 10.64.1.222/30 dev eth0
ip link set eth0 up

# ------- A7 (/29) belakang Switch3: Vilya + Narya -------
# Network: 10.64.1.224/29 → host 10.64.1.225–10.64.1.230
# Rivendell eth1 = 10.64.1.225 (gateway lokal)
ip addr add 10.64.1.225/29 dev eth1
ip link set eth1 up

# Aktifkan routing
echo 1 > /proc/sys/net/ipv4/ip_forward

# Default route ke Osgiliath
ip route add default via 10.64.1.221

exit 0

```

### Osgiliath
```
# JARINGAN BELAKANG RIVENDELL (Vilya + Narya, 10.64.1.224/29)
ip route add 10.64.1.224/29 via 10.64.1.222
```

### Vilya
```
#!/bin/sh

ip addr flush dev eth0
ip addr add 10.64.1.226/29 dev eth0
ip link set eth0 up

ip route add default via 10.64.1.225

echo "nameserver 8.8.8.8" > /etc/resolv.conf
echo "nameserver 1.1.1.1" >> /etc/resolv.conf

exit 0

```

### Narya
```
#!/bin/sh

ip addr flush dev eth0
ip addr add 10.64.1.227/29 dev eth0
ip link set eth0 up

ip route add default via 10.64.1.225

echo "nameserver 8.8.8.8" > /etc/resolv.conf
echo "nameserver 1.1.1.1" >> /etc/resolv.conf

exit 0

```

### Testing
```
ping 10.64.1.221      # Osgiliath
ping 10.64.1.225   # Rivendell
ping 8.8.8.8
ping google.com
```

## Setup Seluruh hal yang Diperlukan

## Jangan Lupa tambahkan (Agar Terhubung ke Internet)
```
nano /etc/rc.local

echo "nameserver 8.8.8.8"  > /etc/resolv.conf
echo "nameserver 8.8.4.4" >> /etc/resolv.conf
echo "nameserver 1.1.1.1" >> /etc/resolv.conf

/etc/rc.local
```

## Vilya as a DHCP Server
```
apt update
apt install isc-dhcp-server -y
```

```
nano /etc/default/isc-dhcp-server

INTERFACESv4="eth0"
INTERFACESv6=""
```

```
nano /etc/dhcp/dhcpd.conf

authoritative;
default-lease-time 600;
max-lease-time 7200;

option domain-name "lotr.local";
# DNS kita: Narya
option domain-name-servers 10.64.1.227;

# ===== A4: Khamul (5 host), 10.64.1.192/29 =====
subnet 10.64.1.192 netmask 255.255.255.248 {
  range 10.64.1.194 10.64.1.198;       # jangan pakai .193 kalau itu IP router
  option routers 10.64.1.193;          # gateway di Winderland
  option broadcast-address 10.64.1.199;
}

# ===== A3: Durin (50 host), 10.64.1.128/26 =====
subnet 10.64.1.128 netmask 255.255.255.192 {
  range 10.64.1.130 10.64.1.190;
  option routers 10.64.1.129;          # gateway di Winderland
  option broadcast-address 10.64.1.191;
}

# ===== A10: Elendil + Isildur (200 + 30 host), 10.64.0.0/24 =====
subnet 10.64.0.0 netmask 255.255.255.0 {
  range 10.64.0.10 10.64.0.250;
  option routers 10.64.0.1;            # gateway di Minastir / Switch4
  option broadcast-address 10.64.0.255;
}

# ===== A13: Gilgalad + Cirdan (100 + 20 host), 10.64.1.0/25 =====
subnet 10.64.1.0 netmask 255.255.255.128 {
  range 10.64.1.10 10.64.1.120;
  option routers 10.64.1.1;            # gateway di AnduinBanks / Switch5
  option broadcast-address 10.64.1.127;
}

# ===== A7: jaringan kecil di belakang Rivendell (Vilya + Narya), 10.64.1.224/29 =====
# Sebenarnya ini dipakai server, tapi kita definisikan juga supaya dhcpd tahu jaringan ini.
subnet 10.64.1.224 netmask 255.255.255.248 {
  range 10.64.1.228 10.64.1.229;       # optional, bisa dipakai host lain kalau ada
  option routers 10.64.1.225;          # gateway = Rivendell
  option broadcast-address 10.64.1.231;
}

service isc-dhcp-server restart
service isc-dhcp-server status
```

## DHCP Relay

### Minastir
```
apt update
apt install isc-dhcp-relay -y
```

```
nano /etc/default/isc-dhcp-relay

SERVERS="10.64.1.226"

# eth2 = ke Switch4 (klien 10.64.0.0/24)
# eth0/eth1 = ke Osgiliath / Pelargir
INTERFACES="eth2 eth0 eth1"

OPTIONS=""

```

```
service isc-dhcp-relay restart
```

### AnduinBanks
```
apt update
apt install isc-dhcp-relay -y
```

```
nano /etc/default/isc-dhcp-relay

SERVERS="10.64.1.226"

# eth1 = ke Switch5 (klien 10.64.1.0/25)
# eth0 = ke Pelargir
INTERFACES="eth1 eth0"

OPTIONS=""

```

```
service isc-dhcp-relay restart
```

### Rivendell
```
apt update
apt install isc-dhcp-relay -y
```

```
SERVERS="10.64.1.226"

# eth1 = ke Switch3 (Vilya/Narya)
# eth0 = ke Osgiliath
INTERFACES="eth1 eth0"

OPTIONS=""
```

```
service isc-dhcp-relay restart
```

## Narya as DNS Server

```
apt update
apt install bind9 -y
```

```
nano /etc/bind/named.conf.options

options {
    directory "/var/cache/bind";

    recursion yes;
    allow-query { any; };

    forwarders {
        8.8.8.8;
        1.1.1.1;
    };

    dnssec-validation auto;

    listen-on-v6 { any; };
};

```

```
ln -s /etc/init.d/named /etc/init.d/bind9
service bind9 restart
```

### Testing

```
dig google.com @127.0.0.1
ping google.com
```

<img width="799" height="704" alt="image" src="https://github.com/user-attachments/assets/3a082f13-f760-41e6-a97b-f916a95d2f54" />

## Web Server

### IronHills
```
apt update
apt install apache2 -y
echo "Welcome to IronHills" > /var/www/html/index.html

```

```
service apache2 start
service apache2 restart
```

### Palantir 

```
apt update
apt install apache2 -y
echo "Welcome to Palantir" > /var/www/html/index.html
```

```
service apache2 start
service apache2 restart
```

## DHCP Client ( Durin - Khamul - Elendil - Ishildur - Gilgalad - Cirdan )

```
nano /etc/rc.local

echo "nameserver 8.8.8.8"  > /etc/resolv.conf
echo "nameserver 8.8.4.4" >> /etc/resolv.conf
echo "nameserver 1.1.1.1" >> /etc/resolv.conf

/etc/rc.local
```

```
nano /etc/network/interfaces

auto eth0
iface eth0 inet dhcp
ifdown eth0 2>/dev/null; ifup eth0
```

### Untuk memanggil lewat host
```
nano /etc/hosts

10.64.1.234  Palantir
10.64.1.210  IronHills
```

### Testing

```
curl http://10.64.1.234
curl http://Palantir
curl http://10.64.1.210
curl http://IronHills
```

<img width="433" height="181" alt="image" src="https://github.com/user-attachments/assets/54efb92d-b205-4bcf-866f-f8d710dce845" />

## Misi 2 No 2 

### Tambahkan ke Osgiriath
```
iptables -A FORWARD -p icmp -d 10.64.1.226 -j DROP
```

```
#!/bin/sh
# rc.local OSGILIATH
# Router pusat + Gateway Internet

#############################################
# 1. IP FORWARDING
#############################################
echo 1 > /proc/sys/net/ipv4/ip_forward


#############################################
# 2. IP ADDRESS INTERFACE INTERNAL (10.64.x.x)
#############################################

# Bersihkan dulu supaya tidak dobel
ip addr flush dev eth1 2>/dev/null
ip addr flush dev eth2 2>/dev/null
ip addr flush dev eth3 2>/dev/null

# A5 – Osgiliath ↔ Moria
ip addr add 10.64.1.218/30 dev eth1

# A6 – Osgiliath ↔ Rivendell
ip addr add 10.64.1.221/30 dev eth2

# A8 – Osgiliath ↔ Minastir
ip addr add 10.64.1.201/29 dev eth3

ip link set eth1 up
ip link set eth2 up
ip link set eth3 up


#############################################
# 3. ROUTING INTERNAL (A1–A13)
#############################################

# ----- KIRI (via Moria: 10.64.1.217) -----
ip route add 10.64.1.208/30 via 10.64.1.217 2>/dev/null   # IronHills
ip route add 10.64.1.128/26 via 10.64.1.217 2>/dev/null   # Durin
ip route add 10.64.1.192/29 via 10.64.1.217 2>/dev/null   # Khamul
ip route add 10.64.1.212/30 via 10.64.1.217 2>/dev/null   # Winderland

# ----- KANAN (via Minastir: 10.64.1.202) -----
ip route add 10.64.0.0/24   via 10.64.1.202 2>/dev/null   # Elendil & Isildur
ip route add 10.64.1.228/30 via 10.64.1.202 2>/dev/null   # Minastir–Pelargir
ip route add 10.64.1.232/30 via 10.64.1.202 2>/dev/null   # Pelargir–Palantir
ip route add 10.64.1.236/30 via 10.64.1.202 2>/dev/null   # Pelargir–AnduinBanks
ip route add 10.64.1.0/25   via 10.64.1.202 2>/dev/null   # Gilgalad & Cirdan

# ----- Vilya & Narya (A7) via Rivendell (10.64.1.222) -----
ip route add 10.64.1.224/29 via 10.64.1.222 2>/dev/null   # Rivendell LAN, Vilya, Narya


#############################################
# 4. KONFIGURASI INTERNET (eth0) – NAT GNS3
#############################################

ip addr flush dev eth0 2>/dev/null
ip addr add 192.168.122.100/24 dev eth0
ip link set eth0 up

ip route del default 2>/dev/null
ip route add default via 192.168.122.1 dev eth0

echo "nameserver 8.8.8.8"  > /etc/resolv.conf
echo "nameserver 8.8.4.4" >> /etc/resolv.conf


#############################################
# 5. FIREWALL – NAT TANPA MASQUERADE (SNAT)
#############################################

iptables -t nat -F
iptables -F FORWARD
iptables -P FORWARD ACCEPT

iptables -t nat -A POSTROUTING -o eth0 -j SNAT --to-source 192.168.122.100


#############################################
# 6. IZINKAN TRAFIK ANTAR-LAN & INTERNET
#############################################

# internal ↔ internet
iptables -A FORWARD -i eth1 -o eth0 -j ACCEPT
iptables -A FORWARD -i eth2 -o eth0 -j ACCEPT
iptables -A FORWARD -i eth3 -o eth0 -j ACCEPT
iptables -A FORWARD -i eth0 -o eth1 -j ACCEPT
iptables -A FORWARD -i eth0 -o eth2 -j ACCEPT
iptables -A FORWARD -i eth0 -o eth3 -j ACCEPT

# antar-LAN (kiri–kanan–tengah)
iptables -A FORWARD -i eth1 -o eth2 -j ACCEPT
iptables -A FORWARD -i eth1 -o eth3 -j ACCEPT
iptables -A FORWARD -i eth2 -o eth1 -j ACCEPT
iptables -A FORWARD -i eth2 -o eth3 -j ACCEPT
iptables -A FORWARD -i eth3 -o eth1 -j ACCEPT
iptables -A FORWARD -i eth3 -o eth2 -j ACCEPT


#############################################
# 7. FIREWALL SPESIAL UNTUK VILYA (10.64.1.226)
#############################################
# 7a. SELALU IZINKAN traffic ESTABLISHED / RELATED dulu
iptables -I FORWARD 1 -m state --state ESTABLISHED,RELATED -j ACCEPT

# 7b. BLOK ping baru (echo-request) dari node lain ke Vilya
iptables -I FORWARD 2 -p icmp --icmp-type echo-request -d 10.64.1.226 -j DROP

exit 0

```

```
chmod +x /etc/rc.local
/etc/rc.local
iptables -L FORWARD -n --line-numbers
```

### Testing ( Sebelum ditambahkan )

<img width="607" height="176" alt="image" src="https://github.com/user-attachments/assets/8e864d76-5906-47bc-8462-bda165fdd021" />

<img width="623" height="153" alt="image" src="https://github.com/user-attachments/assets/5e3ae442-a8b9-412a-a503-6d3ae12a7823" />

### Testing ( Setelah ditambahkan )

<img width="911" height="225" alt="image" src="https://github.com/user-attachments/assets/fe5149a0-a634-4993-816f-84cd7b28879a" />

<img width="654" height="117" alt="image" src="https://github.com/user-attachments/assets/3329c326-6a4a-48f4-9b37-a29db8145a60" />

<img width="647" height="117" alt="image" src="https://github.com/user-attachments/assets/6cfaf9f5-c9fe-4dcc-a8c8-a9a6530fc012" />

### Testing Vilya

<img width="861" height="634" alt="image" src="https://github.com/user-attachments/assets/6a3f99ca-8d31-4aeb-a6ba-c530a9eb29c5" />

### Misi 2 No 3

```
# === Misi 2 No. 3: Batasi akses DNS ke Narya ===

# Izinkan DNS hanya dari Vilya ke Narya
iptables -I FORWARD 1 -s 10.64.1.226 -d 10.64.1.227 -p udp --dport 53 -j ACCEPT

# Blok akses DNS dari semua node lain ke Narya
iptables -I FORWARD 2 -d 10.64.1.227 -p udp --dport 53 -j DROP
```

```
#############################################
# 7. FIREWALL SPESIAL UNTUK VILYA (10.64.1.226)
#############################################
# 7a. SELALU IZINKAN traffic ESTABLISHED / RELATED dulu
iptables -I FORWARD 1 -m state --state ESTABLISHED,RELATED -j ACCEPT

# 7b. BLOK ping baru (echo-request) dari node lain ke Vilya
iptables -I FORWARD 2 -p icmp --icmp-type echo-request -d 10.64.1.226 -j DROP

#############################################
# 8. FIREWALL DNS – HANYA VILYA → NARYA
#############################################
# Izinkan DNS (UDP & TCP 53) hanya dari Vilya (10.64.1.226) ke Narya (10.64.1.227)
iptables -I FORWARD 3 -s 10.64.1.226 -d 10.64.1.227 -p udp --dport 53 -j ACCEPT
iptables -I FORWARD 4 -s 10.64.1.226 -d 10.64.1.227 -p tcp --dport 53 -j ACCEPT

# Blok semua akses DNS (UDP & TCP 53) lain ke Narya
iptables -I FORWARD 5 -d 10.64.1.227 -p udp --dport 53 -j DROP
iptables -I FORWARD 6 -d 10.64.1.227 -p tcp --dport 53 -j DROP

```

```
chmod +x /etc/rc.local
/etc/rc.local
iptables -L FORWARD -n --line-numbers
```

### Testing Vilya ( SUKSES )

<img width="1215" height="400" alt="image" src="https://github.com/user-attachments/assets/353759a2-d27b-4e03-915c-6455d49f7c81" />

```
apt install netcat-openbsd -y

dig google.com @10.64.1.227

nc -vz 10.64.1.227 53
```

<img width="766" height="602" alt="image" src="https://github.com/user-attachments/assets/5686d49d-0972-4bac-ade4-e2f0bf72deec" />


### Testing Client ( Durin ) [GAGAL]
```

apt install netcat-openbsd -y
dig google.com @10.64.1.227

nc -vz 10.64.1.227 53
nc -vz -w 5 10.64.1.227 53
```

<img width="528" height="47" alt="image" src="https://github.com/user-attachments/assets/6aa195aa-b6bb-407a-b806-1a8e8ad77ef2" />

<img width="401" height="58" alt="image" src="https://github.com/user-attachments/assets/772f7c74-a2cc-4598-9a43-ae824d195e82" />

<img width="780" height="78" alt="image" src="https://github.com/user-attachments/assets/32a1bcf8-14f6-4651-86d5-2ab68807c001" />

## Misi 2 No 4

### IronHills
```
#!/bin/sh
# rc.local IRONHILLS
# Web Server + Firewall Akses Terjadwal


#############################################
# 0. MODE AKSES
#############################################
#   PILIH SALAH SATU:
#   weekend_only  = Akses HANYA Sabtu & Minggu
#   weekdays_only = Akses HANYA Senin–Jumat
#############################################

MODE="weekend_only"   # <--- UBAH KE "weekdays_only" kalau perlu saat demo



#############################################
# 1. IP & ROUTING
#############################################

ip addr flush dev eth0 2>/dev/null

# IP IronHills
ip addr add 10.64.1.210/30 dev eth0
ip link set eth0 up

# Default route via Moria
ip route del default 2>/dev/null
ip route add default via 10.64.1.209 dev eth0


#############################################
# 2. DNS
#############################################
echo "nameserver 8.8.8.8"  > /etc/resolv.conf
echo "nameserver 8.8.4.4" >> /etc/resolv.conf


#############################################
# 3. FIREWALL DASAR
#############################################

iptables -F INPUT
iptables -P INPUT ACCEPT

iptables -A INPUT -i lo -j ACCEPT
iptables -A INPUT -m state --state ESTABLISHED,RELATED -j ACCEPT
iptables -A INPUT -p icmp -j ACCEPT
iptables -A INPUT -p tcp --dport 22 -j ACCEPT


#############################################
# 4. FIREWALL WAKTU (HTTP)
#############################################

# IP yang diizinkan
DURIN="10.64.1.130"
KHAMUL="10.64.1.194"
ELENDIL="10.64.0.2"
ISILDUR="10.64.0.3"

case "$MODE" in

    "weekend_only")
        echo "[IRONHILLS] MODE = weekend_only (HANYA Sat,Sun boleh)"

        iptables -A INPUT -p tcp -s $DURIN   --dport 80 -m time --weekdays Sat,Sun --kerneltz -j ACCEPT
        iptables -A INPUT -p tcp -s $KHAMUL  --dport 80 -m time --weekdays Sat,Sun --kerneltz -j ACCEPT
        iptables -A INPUT -p tcp -s $ELENDIL --dport 80 -m time --weekdays Sat,Sun --kerneltz -j ACCEPT
        iptables -A INPUT -p tcp -s $ISILDUR --dport 80 -m time --weekdays Sat,Sun --kerneltz -j ACCEPT
        ;;

    "weekdays_only")
        echo "[IRONHILLS] MODE = weekdays_only (HANYA Mon–Fri boleh)"

        iptables -A INPUT -p tcp -s $DURIN   --dport 80 -m time --weekdays Mon,Tue,Wed,Thu,Fri --kerneltz -j ACCEPT
        iptables -A INPUT -p tcp -s $KHAMUL  --dport 80 -m time --weekdays Mon,Tue,Wed,Thu,Fri --kerneltz -j ACCEPT
        iptables -A INPUT -p tcp -s $ELENDIL --dport 80 -m time --weekdays Mon,Tue,Wed,Thu,Fri --kerneltz -j ACCEPT
        iptables -A INPUT -p tcp -s $ISILDUR --dport 80 -m time --weekdays Mon,Tue,Wed,Thu,Fri --kerneltz -j ACCEPT
        ;;

    *)
        echo "[IRONHILLS] MODE tidak dikenal — tidak ada rule waktu"
        ;;
esac

# Semua akses HTTP lainnya diblok
iptables -A INPUT -p tcp --dport 80 -j REJECT --reject-with icmp-port-unreachable


#############################################
# 5. END
#############################################
exit 0
```

```
service apache2 status
# kalau inactive / failed, hidupkan:
service apache2 start

# kalau mau yakin:
ss -lnpt | grep :80
# harus muncul sesuatu seperti:
# LISTEN 0 128 0.0.0.0:80 ... apache2
```

```
chmod +x /etc/rc.local
/etc/rc.local
iptables -A INPUT -p tcp --dport 80 -j REJECT --reject-with icmp-port-unreachable
```

### Tes di Durin atau Node client manapun

```
curl -v http://10.64.1.210
```

## Misi 2 No 5

### Palantir
```
nano /etc/rc.local

#!/bin/sh
# rc.local PALANTIR
# Server Latihan + Firewall Akses Terjadwal

#############################################
# 1. IP ADDRESS & ROUTING
#############################################

ip addr flush dev eth0 2>/dev/null
ip addr add 10.64.1.234/30 dev eth0
ip link set eth0 up

ip route del default 2>/dev/null
ip route add default via 10.64.1.233 dev eth0

echo "nameserver 8.8.8.8"  > /etc/resolv.conf
echo "nameserver 8.8.4.4" >> /etc/resolv.conf


#############################################
# 2. FIREWALL DASAR
#############################################

iptables -F INPUT
iptables -P INPUT ACCEPT

iptables -A INPUT -i lo -j ACCEPT
iptables -A INPUT -m state --state ESTABLISHED,RELATED -j ACCEPT
iptables -A INPUT -p icmp -j ACCEPT
iptables -A INPUT -p tcp --dport 22 -j ACCEPT


#############################################
# 3. FIREWALL WAKTU PALANTIR (HTTP PORT 80)
#############################################
# Faksi Elf 00:00–16:59
iptables -A INPUT -p tcp -s 10.64.1.10   --dport 80 \
         -m time --timestart 00:00 --timestop 16:59 --kerneltz -j ACCEPT   # Gilgalad
iptables -A INPUT -p tcp -s 10.64.1.11   --dport 80 \
         -m time --timestart 00:00 --timestop 16:59 --kerneltz -j ACCEPT   # Cirdan

# Faksi Manusia 17:00–23:00
iptables -A INPUT -p tcp -s 10.64.0.2    --dport 80 \
         -m time --timestart 17:00 --timestop 23:00 --kerneltz -j ACCEPT   # Elendil
iptables -A INPUT -p tcp -s 10.64.0.3    --dport 80 \
         -m time --timestart 17:00 --timestop 23:00 --kerneltz -j ACCEPT   # Isildur

# Semua selain waktu & IP di atas = TOLAK
iptables -A INPUT -p tcp --dport 80 -j REJECT --reject-with icmp-port-unreachable


#############################################
# 4. SELESAI
#############################################
echo "[PALANTIR] Firewall jadwal AKTIF"
exit 0

```

```
chmod +x /etc/rc.local
/etc/rc.local
```

### Testing ( Sekarang jam 07.31 ) 

<img width="344" height="253" alt="image" src="https://github.com/user-attachments/assets/1a27cf97-6abe-40d8-95fb-a3b0ad301a1b" />

### Gilgalad

<img width="399" height="41" alt="image" src="https://github.com/user-attachments/assets/547baa1f-357c-4147-bbd0-a5b1b5733f74" />

### Elendil

<img width="920" height="241" alt="image" src="https://github.com/user-attachments/assets/c810131a-43f3-4087-a1aa-cea703b8afd7" />

## Misi 2 No 6

### Palantir 
```
nano /etc/rc.local

#!/bin/sh
# rc.local PALANTIR FINAL
# Firewall Jadwal + Anti Port Scan (No log file required)

#############################################
# 1. IP ADDRESS & ROUTING
#############################################

ip addr flush dev eth0 2>/dev/null
ip addr add 10.64.1.234/30 dev eth0
ip link set eth0 up

ip route del default 2>/dev/null
ip route add default via 10.64.1.233 dev eth0

echo "nameserver 8.8.8.8"  > /etc/resolv.conf
echo "nameserver 8.8.4.4" >> /etc/resolv.conf


#############################################
# 2. SIAPKAN CHAIN PORT_SCAN
#############################################

# Hapus chain lama
iptables -F PORT_SCAN 2>/dev/null
iptables -X PORT_SCAN 2>/dev/null

# Buat chain baru
iptables -N PORT_SCAN

# Isi chain
iptables -A PORT_SCAN -m limit --limit 3/min --limit-burst 5 \
    -j LOG --log-prefix "PORT_SCAN_DETECTED: " --log-level 4

iptables -A PORT_SCAN -m recent --set --name blocklist --rsource
iptables -A PORT_SCAN -j DROP


#############################################
# 3. FIREWALL INPUT DASAR
#############################################

iptables -F INPUT
iptables -P INPUT ACCEPT

# PRIORITAS BAN PALING ATAS
iptables -I INPUT 1 -m recent --rcheck --name blocklist --rsource -j DROP

# Loopback & Established
iptables -A INPUT -i lo -j ACCEPT
iptables -A INPUT -m state --state ESTABLISHED,RELATED -j ACCEPT

# ICMP (ping) – aman karena blocklist di rule 1
iptables -A INPUT -p icmp -j ACCEPT

# SSH Selalu boleh
iptables -A INPUT -p tcp --dport 22 -j ACCEPT


#############################################
# 4. DETEKSI PORT SCAN RANGE 1–100
#############################################

# Jika port yang disentuh >= 16 dalam 20 detik → kirim ke PORT_SCAN
iptables -A INPUT -p tcp --syn --dport 1:100 \
    -m recent --update --seconds 20 --hitcount 16 --name portscan --rsource \
    -j PORT_SCAN

# Setiap SYN baru tambahkan ke daftar "portscan"
iptables -A INPUT -p tcp --syn --dport 1:100 \
    -m recent --set --name portscan --rsource


#############################################
# 5. FIREWALL WAKTU PALANTIR (PORT 80)
#############################################

# ELF (Gilgalad 10.64.1.10, Cirdan 10.64.1.11) — 00:00–16:59
iptables -A INPUT -p tcp -s 10.64.1.10 --dport 80 \
    -m time --timestart 00:00 --timestop 16:59 --kerneltz -j ACCEPT
iptables -A INPUT -p tcp -s 10.64.1.11 --dport 80 \
    -m time --timestart 00:00 --timestop 16:59 --kerneltz -j ACCEPT

# MANUSIA (Elendil 10.64.0.2, Isildur 10.64.0.3) — 17:00–23:00
iptables -A INPUT -p tcp -s 10.64.0.2 --dport 80 \
    -m time --timestart 17:00 --timestop 23:00 --kerneltz -j ACCEPT
iptables -A INPUT -p tcp -s 10.64.0.3 --dport 80 \
    -m time --timestart 17:00 --timestop 23:00 --kerneltz -j ACCEPT

# Selain waktu + IP → tolak
iptables -A INPUT -p tcp --dport 80 -j REJECT --reject-with icmp-port-unreachable


#############################################
# 6. INFO
#############################################

echo "[PALANTIR] Firewall jadwal + Anti port scan AKTIF"
iptables -L INPUT -n --line-numbers
iptables -L PORT_SCAN -n --line-numbers

exit 0
```

```
chmod +x /etc/rc.local
/etc/rc.local

Cek
iptables -L INPUT -n --line-numbers
iptables -L PORT_SCAN -n --line-numbers
```

### Elendil ( Sebelum Serangan ) 

```
ping -c 3 10.64.1.234
```

<img width="775" height="536" alt="image" src="https://github.com/user-attachments/assets/30ff28e0-7899-4801-bdfa-ee289a91c8f7" />

### Waktunya Serangan 

```
nmap -p1-100 -T4 10.64.1.234
```

### Elendil ( Setelah Serangan )
```
ping -c 3 10.64.1.234
# 100% packet loss

curl -v http://10.64.1.234
# Connection refused / hang

nc -vz 10.64.1.234 80
# failed
```

<img width="630" height="198" alt="image" src="https://github.com/user-attachments/assets/901b5449-8dde-4fc2-95f4-5747aa359250" />

### Bukti di Palantir
```
cat /proc/net/xt_recent/blocklist
iptables -L PORT_SCAN -n --line-numbers
```

<img width="1339" height="154" alt="image" src="https://github.com/user-attachments/assets/1a2781d2-c996-48ef-9ad6-a473cc1dd555" />

### Jika Mau melakukan Serangan lagi ( Reset ) | Palantir

```
nano /root/reset-portscan.sh

#!/bin/sh
# Reset blacklist port-scan PALANTIR (pakai xt_recent "echo /")

echo "===================================="
echo " RESET PORTSCAN PALANTIR (xt_recent)"
echo "===================================="

# Bersihin daftar IP yang diblokir karena port scan
if [ -f /proc/net/xt_recent/blocklist ]; then
    echo / > /proc/net/xt_recent/blocklist
    echo "[OK] /proc/net/xt_recent/blocklist dibersihkan"
else
    echo "[SKIP] blocklist tidak ada"
fi

if [ -f /proc/net/xt_recent/portscan ]; then
    echo / > /proc/net/xt_recent/portscan
    echo "[OK] /proc/net/xt_recent/portscan dibersihkan"
else
    echo "[SKIP] portscan tidak ada"
fi

# Reload firewall dari rc.local biar rules balik rapi
if [ -x /etc/rc.local ]; then
    echo "[INFO] Menjalankan ulang /etc/rc.local ..."
    /etc/rc.local
else
    echo "[WARN] /etc/rc.local tidak bisa dieksekusi"
fi

echo "===================================="
echo " SELESAI — Palantir siap dites lagi"
echo "===================================="

chmod +x /root/reset-portscan.sh
/root/reset-portscan.sh
```

```
cat /proc/net/xt_recent/blocklist
cat /proc/net/xt_recent/portscan
```

### Tes Lagi Di Erendil
```
ping 10.64.1.234
nmap -p1-100 10.64.1.234
curl -v http://10.64.1.234
```

## Misi 2 No 7

### IronHills
```
#!/bin/sh
# rc.local IRONHILLS
# Web Server + Firewall Akses Terjadwal + Limit 3 koneksi/IP


#############################################
# 0. MODE AKSES
#############################################
#   PILIH SALAH SATU:
#   weekend_only  = Akses HANYA Sabtu & Minggu
#   weekdays_only = Akses HANYA Senin–Jumat
#############################################

MODE="weekdays_only"   # UBAH ke "weekend_only" kalau mau mode Sabtu–Minggu saat demo



#############################################
# 1. IP & ROUTING
#############################################

ip addr flush dev eth0 2>/dev/null

# IP IronHills
ip addr add 10.64.1.210/30 dev eth0
ip link set eth0 up

# Default route via Moria
ip route del default 2>/dev/null
ip route add default via 10.64.1.209 dev eth0



#############################################
# 2. DNS
#############################################
echo "nameserver 8.8.8.8"  > /etc/resolv.conf
echo "nameserver 8.8.4.4" >> /etc/resolv.conf



#############################################
# 3. FIREWALL DASAR
#############################################

iptables -F INPUT
iptables -P INPUT ACCEPT

# Loopback
iptables -A INPUT -i lo -j ACCEPT

# Koneksi yang sudah ESTABLISHED/RELATED
iptables -A INPUT -m state --state ESTABLISHED,RELATED -j ACCEPT

# Ping
iptables -A INPUT -p icmp -j ACCEPT

# SSH
iptables -A INPUT -p tcp --dport 22 -j ACCEPT



#############################################
# 4. LIMIT 3 KONEKSI AKTIF PER IP KE PORT 80
#############################################
# Rule ini berlaku untuk SEMUA IP yang ke port 80.
# Bedanya:
#   - IP yang diizinkan oleh rule waktu (Durin, Khamul, Elendil, Isildur)
#     boleh sampai 3 koneksi paralel.
#   - Koneksi ke-4 dan seterusnya dari IP yang sama: REJECT dengan TCP RST.

iptables -A INPUT -p tcp --syn --dport 80 \
         -m connlimit --connlimit-above 3 --connlimit-mask 32 \
         -j REJECT --reject-with tcp-reset



#############################################
# 5. FIREWALL WAKTU (HTTP)
#############################################

# IP yang diizinkan
DURIN="10.64.1.130"
KHAMUL="10.64.1.194"
ELENDIL="10.64.0.2"
ISILDUR="10.64.0.3"

case "$MODE" in

    "weekend_only")
        echo "[IRONHILLS] MODE = weekend_only (HANYA Sat,Sun boleh)"

        iptables -A INPUT -p tcp -s $DURIN   --dport 80 \
                 -m time --weekdays Sat,Sun --kerneltz -j ACCEPT
        iptables -A INPUT -p tcp -s $KHAMUL  --dport 80 \
                 -m time --weekdays Sat,Sun --kerneltz -j ACCEPT
        iptables -A INPUT -p tcp -s $ELENDIL --dport 80 \
                 -m time --weekdays Sat,Sun --kerneltz -j ACCEPT
        iptables -A INPUT -p tcp -s $ISILDUR --dport 80 \
                 -m time --weekdays Sat,Sun --kerneltz -j ACCEPT
        ;;

    "weekdays_only")
        echo "[IRONHILLS] MODE = weekdays_only (HANYA Mon–Fri boleh)"

        iptables -A INPUT -p tcp -s $DURIN   --dport 80 \
                 -m time --weekdays Mon,Tue,Wed,Thu,Fri --kerneltz -j ACCEPT
        iptables -A INPUT -p tcp -s $KHAMUL  --dport 80 \
                 -m time --weekdays Mon,Tue,Wed,Thu,Fri --kerneltz -j ACCEPT
        iptables -A INPUT -p tcp -s $ELENDIL --dport 80 \
                 -m time --weekdays Mon,Tue,Wed,Thu,Fri --kerneltz -j ACCEPT
        iptables -A INPUT -p tcp -s $ISILDUR --dport 80 \
                 -m time --weekdays Mon,Tue,Wed,Thu,Fri --kerneltz -j ACCEPT
        ;;

    *)
        echo "[IRONHILLS] MODE tidak dikenal — TIDAK ada rule waktu khusus HTTP"
        ;;
esac

# Semua akses HTTP lain (di luar IP/waktu di atas) ditolak
iptables -A INPUT -p tcp --dport 80 -j REJECT --reject-with icmp-port-unreachable



#############################################
# 6. FINISH
#############################################
echo "[IRONHILLS] rc.local selesai"
exit 0
```

```
chmod +x /etc/rc.local
/etc/rc.local
iptables -L INPUT -n --line-numbers
```

### Install Apache Di IronHills

```
apt-get update
apt-get install apache2 -y

# Isi halaman test
echo "Welcome to IronHills" > /var/www/html/index.html

# Start Apache
service apache2 start 2>/dev/null || /etc/init.d/apache2 start

# Cek listen di port 80
ss -tlnp | grep ':80' || netstat -tlnp | grep ':80'
```

### Testing IronHills
```
curl http://127.0.0.1/
curl http://10.64.1.210/
# Harus keluar: Welcome to IronHills
```

### Install ab di Durin (untuk stress test)
```
apt-get update
apt-get install apache2-utils -y

ab -V   # cuma cek versi
```

```
curl http://10.64.1.210
```

### Uji Beban
```
ab -n 3 -c 3 http://10.64.1.210/

curl http://10.64.1.210
curl http://10.64.1.210
curl http://10.64.1.210

TES OVERLOAD
ab -n 20 -c 10 http://10.64.1.210/
ab -n 10 -c 5 http://10.64.1.210/

for i in {1..10}; do
  curl -s http://10.64.1.210/ > /dev/null &
done
wait
```

<img width="891" height="689" alt="image" src="https://github.com/user-attachments/assets/7b7d1a05-ba82-4405-8d10-2f643889f114" />


## MISI 2 NO 8

### Osgiliath
```
#!/bin/sh
# rc.local OSGILIATH
# Router pusat + Gateway Internet

#############################################
# 1. IP FORWARDING
#############################################
echo 1 > /proc/sys/net/ipv4/ip_forward


#############################################
# 2. IP ADDRESS INTERFACE INTERNAL (10.64.x.x)
#############################################

# Bersihkan dulu supaya tidak dobel
ip addr flush dev eth1 2>/dev/null
ip addr flush dev eth2 2>/dev/null
ip addr flush dev eth3 2>/dev/null

# A5 – Osgiliath ↔ Moria
ip addr add 10.64.1.218/30 dev eth1

# A6 – Osgiliath ↔ Rivendell
ip addr add 10.64.1.221/30 dev eth2

# A8 – Osgiliath ↔ Minastir
ip addr add 10.64.1.201/29 dev eth3

ip link set eth1 up
ip link set eth2 up
ip link set eth3 up


#############################################
# 3. ROUTING INTERNAL (A1–A13)
#############################################

# ----- KIRI (via Moria: 10.64.1.217) -----
ip route add 10.64.1.208/30 via 10.64.1.217 2>/dev/null   # IronHills
ip route add 10.64.1.128/26 via 10.64.1.217 2>/dev/null   # Durin
ip route add 10.64.1.192/29 via 10.64.1.217 2>/dev/null   # Khamul
ip route add 10.64.1.212/30 via 10.64.1.217 2>/dev/null   # Winderland

# ----- KANAN (via Minastir: 10.64.1.202) -----
ip route add 10.64.0.0/24   via 10.64.1.202 2>/dev/null   # Elendil & Isildur
ip route add 10.64.1.228/30 via 10.64.1.202 2>/dev/null   # Minastir–Pelargir
ip route add 10.64.1.232/30 via 10.64.1.202 2>/dev/null   # Pelargir–Palantir
ip route add 10.64.1.236/30 via 10.64.1.202 2>/dev/null   # Pelargir–AnduinBanks
ip route add 10.64.1.0/25   via 10.64.1.202 2>/dev/null   # Gilgalad & Cirdan

# ----- Vilya & Narya (A7) via Rivendell (10.64.1.222) -----
ip route add 10.64.1.224/29 via 10.64.1.222 2>/dev/null   # Rivendell LAN, Vilya, Narya


#############################################
# 4. KONFIGURASI INTERNET (eth0) – NAT GNS3
#############################################

ip addr flush dev eth0 2>/dev/null
ip addr add 192.168.122.100/24 dev eth0
ip link set eth0 up

ip route del default 2>/dev/null
ip route add default via 192.168.122.1 dev eth0

echo "nameserver 8.8.8.8"  > /etc/resolv.conf
echo "nameserver 8.8.4.4" >> /etc/resolv.conf


#############################################
# 5. FIREWALL – NAT TANPA MASQUERADE (SNAT)
#############################################

iptables -t nat -F
iptables -F FORWARD
iptables -P FORWARD ACCEPT

# NAT ke internet (GNS3 cloud)
iptables -t nat -A POSTROUTING -o eth0 -j SNAT --to-source 192.168.122.100


#############################################
# 6. IZINKAN TRAFIK ANTAR-LAN & INTERNET
#############################################

# internal ↔ internet
iptables -A FORWARD -i eth1 -o eth0 -j ACCEPT
iptables -A FORWARD -i eth2 -o eth0 -j ACCEPT
iptables -A FORWARD -i eth3 -o eth0 -j ACCEPT
iptables -A FORWARD -i eth0 -o eth1 -j ACCEPT
iptables -A FORWARD -i eth0 -o eth2 -j ACCEPT
iptables -A FORWARD -i eth0 -o eth3 -j ACCEPT

# antar-LAN (kiri–kanan–tengah)
iptables -A FORWARD -i eth1 -o eth2 -j ACCEPT
iptables -A FORWARD -i eth1 -o eth3 -j ACCEPT
iptables -A FORWARD -i eth2 -o eth1 -j ACCEPT
iptables -A FORWARD -i eth2 -o eth3 -j ACCEPT
iptables -A FORWARD -i eth3 -o eth1 -j ACCEPT
iptables -A FORWARD -i eth3 -o eth2 -j ACCEPT


#############################################
# 7. FIREWALL SPESIAL UNTUK VILYA (10.64.1.226)
#############################################
# 7a. SELALU IZINKAN traffic ESTABLISHED / RELATED dulu
iptables -I FORWARD 1 -m state --state ESTABLISHED,RELATED -j ACCEPT

# 7b. BLOK ping baru (echo-request) dari node lain ke Vilya
iptables -I FORWARD 2 -p icmp --icmp-type echo-request -d 10.64.1.226 -j DROP


#############################################
# 8. FIREWALL DNS – HANYA VILYA → NARYA
#############################################
# Izinkan DNS (UDP & TCP 53) hanya dari Vilya (10.64.1.226) ke Narya (10.64.1.227)
iptables -I FORWARD 3 -s 10.64.1.226 -d 10.64.1.227 -p udp --dport 53 -j ACCEPT
iptables -I FORWARD 4 -s 10.64.1.226 -d 10.64.1.227 -p tcp --dport 53 -j ACCEPT

# Blok semua akses DNS (UDP & TCP 53) lain ke Narya
iptables -I FORWARD 5 -d 10.64.1.227 -p udp --dport 53 -j DROP
iptables -I FORWARD 6 -d 10.64.1.227 -p tcp --dport 53 -j DROP


#############################################
# 9. SIHIR HITAM: REDIRECT VILYA → KHAMUL → IRONHILLS
#############################################
# Dari Vilya (10.64.1.226) yang MAU ke Khamul (10.64.1.194),
# dibelokkan ke IronHills (10.64.1.210).

# 9a. Ubah tujuan paket: Vilya -> Khamul MENJADI Vilya -> IronHills
iptables -t nat -A PREROUTING \
    -s 10.64.1.226 -d 10.64.1.194 \
    -j DNAT --to-destination 10.64.1.210

# 9b. Balasan dari IronHills ke Vilya disamarkan seolah-olah dari Khamul
iptables -t nat -A POSTROUTING \
    -s 10.64.1.210 -d 10.64.1.226 \
    -j SNAT --to-source 10.64.1.194


#############################################
# 10. SELESAI
#############################################
exit 0
```

```
chmod +x /etc/rc.local
/etc/rc.local

iptables -t nat -L PREROUTING -n --line-numbers
iptables -t nat -L POSTROUTING -n --line-numbers
```

### Di IronHills
```
apt install netcat-openbsd -y
nc -l -p 9999
```

### Di Khamul
```
apt install netcat-openbsd -y
nc -l -p 9999
```

### Di Vilyan
```
echo "Halo dari Vilya" | nc 10.64.1.194 9999
```

<img width="339" height="69" alt="image" src="https://github.com/user-attachments/assets/270ffee6-4f35-411f-b183-40407c3d69bc" />

## MISI 3 NO 1

### Moria
```
# Blok semua trafik KELUAR dari Khamul (ke mana pun)
iptables -I FORWARD 1 -s 10.64.1.192/29 -j DROP

# Blok semua trafik MASUK ke Khamul (dari mana pun)
iptables -I FORWARD 2 -d 10.64.1.192/29 -j DROP
```

```
chmod +x /etc/rc.local
/etc/rc.local
iptables -L FORWARD -n --line-numbers
```

### IronHills

```
ping 10.64.1.194
nc -vz 10.64.1.194 80
```

<img width="683" height="152" alt="image" src="https://github.com/user-attachments/assets/3a8ea630-9fde-440c-b6e3-d71b8891933f" />

### Khamul
```
ping 10.64.1.210
nc -vz 10.64.1.210 80
```

<img width="627" height="155" alt="image" src="https://github.com/user-attachments/assets/240f10eb-e6c8-4fc1-a94b-69409f2ee059" />
