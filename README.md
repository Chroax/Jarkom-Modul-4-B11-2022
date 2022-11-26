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

### Langkah

### Tree

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
![image](https://raw.githubusercontent.com/Chroax/Jarkom-Modul-4-B11-2022/main/image/CIDR/Step/step-5.PNG)

#### Step-6
![image](https://raw.githubusercontent.com/Chroax/Jarkom-Modul-4-B11-2022/main/image/CIDR/Step/step-6.PNG)

#### Step-7
![image](https://raw.githubusercontent.com/Chroax/Jarkom-Modul-4-B11-2022/main/image/CIDR/Step/step-7.PNG)

### CIDR

![image](https://raw.githubusercontent.com/Chroax/Jarkom-Modul-4-B11-2022/main/image/CIDR/CIDR.PNG)

### Tree

![image](https://raw.githubusercontent.com/Chroax/Jarkom-Modul-4-B11-2022/main/image/CIDR/tree.png)

### CIDR-IP

![image](https://raw.githubusercontent.com/Chroax/Jarkom-Modul-4-B11-2022/main/image/CIDR/cidr-ip.PNG)

### Konfigurasi Node

- **ThePerformance**
    ```
    auto lo
    iface lo inet loopback
    
    auto eth0
    iface eth0 inet dhcp
    
    auto eth1
    iface eth1 inet static
    address 192.178.112.1
    netmask 255.255.255.252
    
    auto eth2
    iface eth2 inet static
    address 192.178.98.1
    netmask 255.255.255.252
    
    auto eth3
    iface eth3 inet static
    address 192.178.80.1
    netmask 255.255.255.252
    
    auto eth4
    iface eth4 inet static
    address 192.178.32.1
    netmask 255.255.255.252
    ```

- **TheMagical**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 192.178.98.2
    netmask 255.255.255.252
    gateway 192.178.98.1

    auto eth1
    iface eth1 inet static
    address 192.178.96.1
    netmask 255.255.254.0
    ```

- **TheOrder**
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
    address 192.178.8.1
    netmask 255.255.255.252

    auto eth2
    iface eth2 inet static
    address 10.8.16.1
    netmask 255.255.255.192
    ```

- **TheMinister**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 192.178.8.2
    netmask 255.255.255.252
    gateway 192.178.8.1

    auto eth1
    iface eth1 inet static
    address 192.178.5.1
    netmask 255.255.255.252

    auto eth2
    iface eth2 inet static
    address 192.178.0.1
    netmask 255.255.252.0
    ```

- **TheDauntless**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 192.178.5.2
    netmask 255.255.255.252
    gateway 192.178.5.1

    auto eth1
    iface eth1 inet static
    address 192.178.4.1
    netmask 255.255.255.0
    ```

- **TheInstrument**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 192.178.80.2
    netmask 255.255.255.252
    gateway 192.178.80.1

    auto eth1
    iface eth1 inet static
    address 192.178.73.1
    netmask 255.255.255.252

    auto eth2
    iface eth2 inet static
    address 192.178.68.1
    netmask 255.255.255.252

    auto eth3
    iface eth3 inet static
    address 192.178.76.1
    netmask 255.255.255.128
    ```

- **TheFireFist**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 192.178.68.2
    netmask 255.255.255.252
    gateway 192.178.68.1

    auto eth1
    iface eth1 inet static
    address 192.178.66.1
    netmask 255.255.254.0

    auto eth2
    iface eth2 inet static
    address 192.178.64.1
    netmask 255.255.255.0
    ```

- **TheProfound**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 192.178.73.2
    netmask 255.255.255.252
    gateway 192.178.73.1

    auto eth1
    iface eth1 inet static
    address 192.178.73.1
    netmask 255.255.255.128

    auto eth2
    iface eth2 inet static
    address 192.178.72.129
    netmask 255.255.255.128
    ```

- **TheQueen**
    ```
    auto lo
    iface lo inet loopback

    auto eth0
    iface eth0 inet static
    address 192.178.64.2
    netmask 255.255.255.0
    gateway 192.178.64.1

    auto eth1
    iface eth1 inet static
    address 192.178.65.1
    netmask 255.255.255.252
    ```

- **Haines**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.96.2
    netmask 255.255.254.0
    gateway 192.178.96.1
    ```

- **Corveks**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.96.3
    netmask 255.255.254.0
    gateway 192.178.96.1
    ```

- **TheBeast**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.112.2
    netmask 255.255.255.252
    gateway 192.178.112.1
    ```

- **Ashaf**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.16.2
    netmask 255.255.255.192
    gateway 192.178.16.1
    ```

- **Guidessau**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.0.2
    netmask 255.255.252.0
    gateway 192.178.0.1
    ```

- **Johan**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.4.3
    netmask 255.255.255.0
    gateway 192.178.4.1
    ```

- **Phanora**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.4.2
    netmask 255.255.255.0
    gateway 192.178.4.1
    ```

- **MattCugat**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.76.2
    netmask 255.255.255.128
    gateway 192.178.76.1
    ```

- **Helga**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.72.130
    netmask 255.255.255.128
    gateway 192.178.72.129
    ```

- **Spendrow**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.72.2
    netmask 255.255.255.128
    gateway 192.178.72.1
    ```

- **Oakleave**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.66.2
    netmask 255.255.254.0
    gateway 192.178.66.1
    ```

- **Keith**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.64.3
    netmask 255.255.255.0
    gateway 192.178.64.1
    ```

- **TheWitch**
    ```
    auto eth0
    iface eth0 inet static
    address 192.178.65.2
    netmask 255.255.255.252
    gateway 192.178.65.1

### Konfigurasi Routing

- **ThePerformance**
    ```

    ```

- **TheMagical**
    ```

    ```

- **TheOrder**
    ```

    ```

- **TheMinister**
    ```

    ```

- **TheDauntless**
    ```

    ```

- **TheInstrument**
    ```

    ```

- **TheFireFist**
    ```

    ```

- **TheProfound**
    ```

    ```

- **All Client**
    ```

    ```

## Kendala
