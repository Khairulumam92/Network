Tentukan alamat network, broadcast dan range IP untuk host jika diketahui IP address berikut :
1. 172.17.4.17 netmask 255.255.255.224
a. ubah IP Address serta prefix ke dalam biner
                                            Net <--|--> Host
IP Address  : 1010 1100 . 0001 0001 . 0000 0100 . 0|001 0001
Subnet Mask : 1111 1111 . 1111 1111 . 1111 1111 . 1|110 0000
====================AND=========================
Network     : 1010 1100 . 0001 0001 . 0000 0100 . 0|000 0000 (172.17.4.0)
================================================
Host ke-1   : 1010 1100 . 0001 0001 . 0000 0100 . 0|000 0001 /host pertama pasti berawalan 1
End Host    : 1010 1100 . 0001 0001 . 0000 0100 . 0|111 1110 /End host pasti berakhiran 0
Broadcast   : 1010 1100 . 0001 0001 . 0000 0100 . 0|111 1111 /Broadcast pasti angka 1 semua
============Conv To Decimal============
Host ke-1   : 172.17.4.1
End Host    : 172.17.4.126
Broadcast   : 172.17.4.127
++++++++++=Hasil=++++++++++
IP Range 172.17.4.1 s.d 172.17.4.126
IP Broadcast: 172.17.4.127


2. 172.16.23.25/19
255.255.224.0
                                            Net <--|--> Host
IP Address  : 1010 1100 . 0001 0000 . 0001 0111 . 0|001 1001
Subnet Mask : 1111 1111 . 1111 1111 . 1110 0000 . 0|000 0000
====================AND=========================
Network     : 1010 1100 . 0001 0000 . 0000 0000 . 0|000 0000 (172.16.0.0)
================================================
Networknya tetap sama
Host ke-1   : 1010 1100 . 0001 0000 . 0000 0000 . 0|000 0001 /host pertama pasti berawalan 1
Broadcast   : 1010 1100 . 0001 0000 . 0000 0000 . 0|111 1110 /End host pasti berakhiran 0
End Host    : 1010 1100 . 0001 0000 . 0000 0000 . 0|111 1111 /Broadcast pasti angka 1 semua
============Conv To Decimal============
Host ke-1   : 172.16.0.1
End Host    : 172.16.0.126
Broadcast   : 172.16.0.127
++++++++++=Hasil=++++++++++
IP Range 172.16.0.1 s.d 172.16.0.126
IP Broadcast: 172.16.0.127


3. 192.168.10.101 /28
255.255.255.240
                                            Net <--|--> Host
IP Address  : 1100 0000 . 1010 1000 . 0000 1010 . 0|110 0101
Subnet Mask : 1111 1111 . 1111 1111 . 1111 1111 . 1|111 0000
====================AND========================= 
Network     : 1100 0000 . 1010 1000 . 0000 1010 . 0|110 0000 (192.168.10.96)
================================================
Networknya tetap sama
Host ke-1   : 1100 0000 . 1010 1000 . 0000 1010 . 0|000 0001 /host pertama pasti berawalan 1
End Host    : 1100 0000 . 1010 1000 . 0000 1010 . 0|111 1110 /End host pasti berakhiran 0
Broadcast   : 1100 0000 . 1010 1000 . 0000 1010 . 0|111 1111 /Broadcast pasti angka 1 semua
============Conv To Decimal============
Host ke-1   : 192.168.10.1
End Host    : 192.168.10.126
Broadcast   : 192.168.10.127
++++++++++=Hasil=++++++++++
IP Range 192.168.10.1 s.d 192.168.10.126
IP Broadcast: 192.168.10.127

4. 10.10.7.8 netmask 255.240.0.0
                                            Net <--|--> Host
IP Address  : 0000 1010 . 0000 1010 . 0000 0111 . 0|000 1000
Subnet Mask : 1111 1111 . 1111 0000 . 0000 0000 . 0|000 0000
====================AND========================= 
Network     : 0000 1010 . 0000 0000 . 0000 0000 . 0|000 0000 (10.0.0.0)
================================================
Networknya tetap sama
Host ke-1   : 0000 1010 . 0000 0000 . 0000 0000 . 0|000 0001 /host pertama pasti berawalan 1
End Host    : 0000 1010 . 0000 0000 . 0000 0000 . 0|111 1110 /End host pasti berakhiran 0
Broadcast   : 0000 1010 . 0000 0000 . 0000 0000 . 0|111 1111 /Broadcast pasti angka 1 semua
============Conv To Decimal============
Host ke-1   : 10.0.0.1
End Host    : 10.0.0.126
Broadcast   : 10.0.0.127
++++++++++=Hasil=++++++++++
IP Range 10.0.0.1 s.d 10.0.0.126
IP Broadcast: 10.0.0.127

5. 175.180.19.40 /13
255.248.0.0
                                            Net <--|--> Host
IP Address  : 1010 1111 . 1011 0100 . 0001 0011 . 0|010 1000
Subnet Mask : 1111 1111 . 1111 1000 . 0000 0000 . 0|000 0000
====================AND========================= 
Network     : 1010 1111 . 1011 0000 . 0000 0000 . 0|000 0000 (175.176.0.0)
================================================
Networknya tetap sama
Host ke-1   : 1010 1111 . 1011 0000 . 0000 0000 . 0|000 0001 /host pertama pasti berawalan 1
End Host    : 1010 1111 . 1011 0000 . 0000 0000 . 0|111 1110 /End host pasti berakhiran 0
Broadcast   : 1010 1111 . 1011 0000 . 0000 0000 . 0|111 1111 /Broadcast pasti angka 1 semua
============Conv To Decimal============
Host ke-1   : 175.176.0.1
End Host    : 175.176.0.126
Broadcast   : 175.176.0.127
++++++++++=Hasil=++++++++++
IP Range 175.176.0.1 s.d 175.176.0.126
IP Broadcast: 175.176.0.127