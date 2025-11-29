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
