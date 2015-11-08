**eth** - интерфейсы Ethernet-адаптеров

Просмотр:
~~~
$ ifconfig
$ ifconfig -a
$ ifconfig eth
~~~

Конфигурирование:
~~~
# nano /etc/network/interfaces
~~~
Пример содержимого файла:
~~~
# interfaces(5) file used by ifup(8) and ifdown(8)
# ========================================================================
# lo
# ========================================================================
auto lo
# Always
iface lo inet loopback
# ========================================================================
# eth0
# ========================================================================
auto eth0

# Конфигурация для динамического IP:
# iface eth0 inet dhcp

# Конфигурация для статического IP:
iface eth0 inet static
  address 192.168.1.88
  netmask 255.255.255.0
  gateway 192.168.1.1
  dns-nameservers 8.8.8.8

# auto eth0.5
iface eth0.5 inet static
  address 192.168.1.85
  netmask 255.255.255.0
#  gateway 192.168.1.1
#  dns-nameservers 8.8.8.8

# auto eth0.7
iface eth0.7 inet static
  address 192.168.1.87
  netmask 255.255.255.0
#  gateway 192.168.1.1
#  dns-nameservers 8.8.8.8

~~~

