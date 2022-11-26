# Jarkom-Modul-4-B11-2022

### Kelompok B11

| **No** | **Nama**              | **NRP**    |
| ------ | --------------------- | ---------- |
| 1      | Cahyadi Surya Nugraha | 5025201184 |
| 2      | Sarah Alissa Putri    | 5025201272 |
| 3      | Ravin Pradhitya       | 5025201068 |

### List

1. [VLSM](#VLSM)
2. [CIDR](#CIDR)

## VLSM

### Topologi
Buat topologi jaringan yang sesuai yaitu dengan mengatur IP Address pada setiap interface yang ada.
![soal shift 4 1](https://user-images.githubusercontent.com/81427127/204072322-ff196756-c748-4ae5-a024-d0fa631687dc.png)

### Langkah
Kemudian buat plotting subnettingnya,
![Frame 1](https://user-images.githubusercontent.com/81427127/204072562-157a0bc4-bc25-4afa-87c0-511ccb8215b8.png)
<img width="318" alt="Screenshot_20221126_114804" src="https://user-images.githubusercontent.com/81427127/204072711-7772898b-a19e-4c2a-a386-67eb00b3a18a.png">

### Tree
Setelah dilakukan pembagian subnetting, lakukan pembagian IP Address menggunakan tree pada setiap interface yang ada.
![Tabloid - 1](https://user-images.githubusercontent.com/81427127/204072752-e3a8a67b-47e2-4520-add6-286f3c1f8548.png)

### VLSM-IP

### Testing

## CIDR

### Topologi

![image](https://raw.githubusercontent.com/Chroax/Jarkom-Modul-4-B11-2022/main/image/CIDR/topologi.PNG)

### Topologi-subnet

![image](https://raw.githubusercontent.com/Chroax/Jarkom-Modul-4-B11-2022/main/image/CIDR/topologi-subnet.PNG)

### Langkah

#### Step-1

![image](https://raw.githubusercontent.com/Chroax/Jarkom-Modul-4-B11-2022/main/image/CIDR/Step/step-1.PNG)

#### Step-2
![image](https://raw.githubusercontent.com/Chroax/Jarkom-Modul-4-B11-2022/main/image/CIDR/Step/step-2.PNG)

#### Step-3
![image](https://raw.githubusercontent.com/Chroax/Jarkom-Modul-4-B11-2022/main/image/CIDR/Step/step-3.PNG)

#### Step-4
![image](https://raw.githubusercontent.com/Chroax/Jarkom-Modul-4-B11-2022/main/image/CIDR/Step/step-4.PNG)

#### Step-5
![image](https://raw.githubusercontent.com/Chroax/Jarkom-Modul-4-B11-2022/main/image/CIDR/Step/Step-5.jpg)

#### Step-6
![image](https://raw.githubusercontent.com/Chroax/Jarkom-Modul-4-B11-2022/main/image/CIDR/Step/Step-6.jpg)

#### Step-7
![image](https://raw.githubusercontent.com/Chroax/Jarkom-Modul-4-B11-2022/main/image/CIDR/Step/Step-7.jpg)

#### Step-8
![image](https://raw.githubusercontent.com/Chroax/Jarkom-Modul-4-B11-2022/main/image/CIDR/Step/Step-8.jpg)

#### Step-9
![image](https://raw.githubusercontent.com/Chroax/Jarkom-Modul-4-B11-2022/main/image/CIDR/Step/Step-9.jpg)

#### Step-10
![image](https://raw.githubusercontent.com/Chroax/Jarkom-Modul-4-B11-2022/main/image/CIDR/Step/Step-10.jpg)

### CIDR

![image](https://raw.githubusercontent.com/Chroax/Jarkom-Modul-4-B11-2022/main/image/CIDR/CIDR.PNG)

### Tree

![image](https://raw.githubusercontent.com/Chroax/Jarkom-Modul-4-B11-2022/main/image/CIDR/tree.png)

### Konfigurasi Node

- **ThePerformance**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet dhcp

    auto eth1
    iface eth1 inet static
    address 192.178.68.1
    netmask 255.255.255.252

    auto eth2
    iface eth2 inet static
    address 192.178.66.1
    netmask 255.255.255.252

    auto eth3
    iface eth3 inet static
    address 192.178.32.1
    netmask 255.255.255.252

    auto eth4
    iface eth4 inet static
    address 192.178.160.1
    netmask 255.255.255.252
    ```

- **TheMagical**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 192.178.66.2
    netmask 255.255.255.252
    gateway 192.178.66.1

    auto eth1
    iface eth1 inet static
    address 192.178.64.1
    netmask 255.255.254.0
    ```

- **TheOrder**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 192.178.160.2
    netmask 255.255.255.252
    gateway 192.178.160.1

    auto eth1
    iface eth1 inet static
    address 192.178.136.1
    netmask 255.255.255.252

    auto eth2
    iface eth2 inet static
    address 192.178.144.1
    netmask 255.255.255.192
    ```

- **TheMinister**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 192.178.136.2
    netmask 255.255.255.252
    gateway 192.178.136.1

    auto eth1
    iface eth1 inet static
    address 192.178.133.1
    netmask 255.255.255.252

    auto eth2
    iface eth2 inet static
    address 192.178.128.1
    netmask 255.255.252.0
    ```

- **TheDauntless**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 192.178.133.2
    netmask 255.255.255.252
    gateway 192.178.133.1

    auto eth1
    iface eth1 inet static
    address 192.178.132.1
    netmask 255.255.255.0
    ```

- **TheInstrument**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 192.178.32.2
    netmask 255.255.255.252
    gateway 192.178.32.1

    auto eth1
    iface eth1 inet static
    address 192.178.17.1
    netmask 255.255.255.252

    auto eth2
    iface eth2 inet static
    address 192.178.4.1
    netmask 255.255.255.252

    auto eth3
    iface eth3 inet static
    address 192.178.8.1
    netmask 255.255.255.128
    ```

- **TheFireFist**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 192.178.4.2
    netmask 255.255.255.252
    gateway 192.178.4.1

    auto eth1
    iface eth1 inet static
    address 192.178.2.1
    netmask 255.255.254.0

    auto eth2
    iface eth2 inet static
    address 192.178.0.1
    netmask 255.255.255.0
    ```

- **TheProfound**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 192.178.17.2
    netmask 255.255.255.252
    gateway 192.178.17.1

    auto eth1
    iface eth1 inet static
    address 192.178.16.1
    netmask 255.255.255.128

    auto eth2
    iface eth2 inet static
    address 192.178.16.129
    netmask 255.255.255.128
    ```

- **TheQueen**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 192.178.0.2
    netmask 255.255.255.0
    gateway 192.178.0.1

    auto eth1
    iface eth1 inet static
    address 192.178.1.1
    netmask 255.255.255.252
    ```

- **Haines**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.64.2
    netmask 255.255.254.0
    gateway 192.178.64.1
    ```

- **Corveks**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.64.3
    netmask 255.255.254.0
    gateway 192.178.64.1
    ```

- **TheBeast**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.68.2
    netmask 255.255.255.252
    gateway 192.178.68.1
    ```

- **Ashaf**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.144.2
    netmask 255.255.255.192
    gateway 192.178.144.1
    ```

- **Guidessau**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.128.2
    netmask 255.255.252.0
    gateway 192.178.128.1
    ```

- **Johan**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.132.3
    netmask 255.255.255.0
    gateway 192.178.132.1
    ```

- **Phanora**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.132.2
    netmask 255.255.255.0
    gateway 192.178.132.1
    ```

- **MattCugat**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.8.2
    netmask 255.255.255.128
    gateway 192.178.8.1
    ```

- **Helga**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.16.130
    netmask 255.255.255.128
    gateway 192.178.16.129
    ```

- **Spendrow**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.16.2
    netmask 255.255.255.128
    gateway 192.178.16.1
    ```

- **Oakleave**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.2.2
    netmask 255.255.254.0
    gateway 192.178.2.1
    ```

- **Keith**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.0.3
    netmask 255.255.255.0
    gateway 192.178.0.1
    ```

- **TheWitch**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.1.2
    netmask 255.255.255.252
    gateway 192.178.1.1
    ```
### Konfigurasi Routing

- **ThePerformance**
    ```
    route add -net 192.178.144.0 netmask 255.255.255.192 gw 192.178.160.2
    route add -net 192.178.136.0 netmask 255.255.255.252 gw 192.178.160.2
    route add -net 192.178.128.0 netmask 255.255.252.0 gw 192.178.160.2
    route add -net 192.178.133.0 netmask 255.255.255.252 gw 192.178.160.2
    route add -net 192.178.132.0 netmask 255.255.255.0 gw 192.178.160.2

    route add -net 192.178.64.0 netmask 255.255.254.0 gw 192.178.66.2

    route add -net 192.178.8.0 netmask 255.255.255.128 gw 192.178.32.2
    route add -net 192.178.17.0 netmask 255.255.255.252 gw 192.178.32.2
    route add -net 192.178.16.0 netmask 255.255.255.128 gw 192.178.32.2
    route add -net 192.178.16.128 netmask 255.255.255.128 gw 192.178.32.2
    route add -net 192.178.4.0 netmask 255.255.255.252 gw 192.178.32.2
    route add -net 192.178.2.0 netmask 255.255.254.0 gw 192.178.32.2
    route add -net 192.178.0.0 netmask 255.255.255.0 gw 192.178.32.2
    route add -net 192.178.1.0 netmask 255.255.255.252 gw 192.178.32.2

    iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 192.178.0.0/16
    ```

- **TheMagical**
    ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.178.66.1
    ```

- **TheOrder**
    ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.178.160.1

    route add -net 192.178.128.0 netmask 255.255.252.0 gw 192.178.136.2
    route add -net 192.178.133.0 netmask 255.255.255.252 gw 192.178.136.2
    route add -net 192.178.132.0 netmask 255.255.255.0 gw 192.178.136.2
    ```

- **TheMinister**
    ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.178.136.1

    route add -net 192.178.132.0 netmask 255.255.255.0 gw 192.178.133.2
    ```

- **TheDauntless**
    ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.178.133.1
    ```

- **TheInstrument**
    ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.178.32.1

    route add -net 192.178.16.0 netmask 255.255.255.128 gw 192.178.17.2
    route add -net 192.178.16.128 netmask 255.255.255.128 gw 192.178.17.2

    route add -net 192.178.2.0 netmask 255.255.254.0 gw 192.178.4.2
    route add -net 192.178.0.0 netmask 255.255.255.0 gw 192.178.4.2
    route add -net 192.178.1.0 netmask 255.255.255.252 gw 192.178.4.2
    ```

- **TheFireFist**
    ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.178.4.1

    route add -net 192.178.1.0 netmask 255.255.255.252 gw 192.178.0.2
    ```

- **TheProfound**
    ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.178.17.1
    ```

- **TheQueen**
    ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.178.0.1
    ```

- **All Except ThePerformance**
    ```
    echo nameserver 192.168.122.1 > /etc/resolv.conf
    ```

## Kendala
