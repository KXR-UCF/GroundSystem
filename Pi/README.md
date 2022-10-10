## Installation
* Install Raspbian 64 bit Lite
* SSH into the pi
```bash
sudo apt update
sudo apt upgrade -y
sudo apt install git -y
git clone https://github.com/KXR-UCF/GroundSystem.git

```
## Installing Docker
```
curl -sSL https://get.docker.com | sh
sudo usermod -aG docker pi
sudo reboot
```
Log back into the pi
### Installing Grafana InfluxDB Heimdall Portainer Crongraf
```
sudo apt install docker-compose -y
cd GroundSystem/Pi/Docker
docker-compose up -d
```
Wait for this to complete, may take a few minutes