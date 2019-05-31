# K8PortScan

##Code: https://github.com/k8gege/K8PortScan
##K8portScan 1.0
##Date: 20190530
##Author: K8gege
##Usage:
##IP (IP IP/24 IP/16 IP/8)
##
##python K8PortScan.py -ip 192.11.22.29
##python K8PortScan.py -ip 192.11.22.29 -p 80-89
##python K8PortScan.py -ip 192.11.22.29/24 -p 80,445,3306
##
##IPlist (ip.txt ip24.txt ip16.txt ip8.txt)
##python K8PortScan.py -f ip.txt
##python K8PortScan.py -f ip.txt -p 80-89
##python K8PortScan.py -f ip24.txt -p 80,445,3306

支持A段、B段、C段(单个或IP列表)
可多个端口或端口范围扫描
Banner识别比S加强版更准


IP文件例子：

无论是ip24.txt ip16.txt ip.txt 或是任意文件名比如 sb.log
格式均为ip

例子：

批量C段扫描
ip24.txt 
192.11.22.4 (任意IP自动提取C段192.11.22)
10.1.10.1   (任意IP自动提取C段10.1.10)

批量B段扫描
ip16.txt
192.11.22.8 (任意IP自动提取B段192.11)
10.10.2.5   (任意IP自动提取B段10.10)

批量IP扫描
ip.txt或any.xxx
192.11.22.8
192.11.22.29
10.123.1.2
118.22.55.6
