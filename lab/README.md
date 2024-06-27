# Notes
* The lab was tested on [Kali Linux 2023.4](https://old.kali.org/kali-images/kali-2023.4/kali-linux-2023.4-installer-amd64.iso), also works on Kali Linux 2024.2
* Your Kali machine should have at least 4GB(More than 4GB optimal) of RAM and 40GB of hard disk space.

# Lab Diagram
<p>
  <img src="https://github.com/dolevf/Black-Hat-Bash/blob/master/lab/lab-network-diagram.png?raw=true" width="600px" alt="BHB"/>
</p>

# Lab Machine IP Addreses
| Machine  | Public IP | Private IP | Hostname
| -------- | ------- | ------- | ------- | 
| p-web-01  | 172.16.10.10  |  | p-web-01.acme-infinity-servers.com |
| p-ftp-01  | 172.16.10.11  | | p-ftp-01.acme-infinity-servers.com  |
| p-web-02  | 172.16.10.12  | 10.1.0.11 | p-web-02.acme-infinity-servers.com  |
| p-jumpbox-01 | 172.16.10.13 | 10.1.0.12 | p-jumpbox-01.acme-infinity-servers.com |
| c-backup-01 | | 10.1.0.13 | c-backup-01.acme-infinity-servers.com |
| c-redis-01 | | 10.1.0.14 | c-redis-01.acme-infinity-servers.com |
| c-db-01 | | 10.1.0.15 | c-db-01.acme-infinity-servers.com |
| c-db-02 | | 10.1.0.16 | c-db-02.acme-infinity-servers.com |


# Lab Installation
Clone the lab from the repo below:
[]()

**Note**: These lab instructions were tested on Kali Linux only.


**Start the Docker Service** 

`sudo service docker start`

## Start the Lab
Go into the lab folder in this repository and run:

`sudo make deploy`

## Test the Lab
`sudo make test`

## Stop the Lab
`sudo make teardown`

## Rebuild the Lab
`sudo make rebuild`

## Destroy the Lab
`sudo make clean`

