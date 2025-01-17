cd RuleTestFramework-main
   22  ls
   23  cd Tools/
   24  ls
   25  cd calderaToAttire/
   26  ls
   27* 
   28  git clone https://github.com/improsec/calderaToAttire
   29  sudo git clone https://github.com/improsec/calderaToAttire
   30  ls
   31  cd calderaToAttire/
   32  ls
   33  cat README.md 
   34  cp /home/analyst/Downloads/T210.005_report.json .
   35  sudo cp /home/analyst/Downloads/T210.005_report.json .
   36  ls
   37  sudo python3 CalderaToAttire.py T210.005_report.json
   38  ls
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    2  cd /opt/Tools
    3  cd /opt
    4  ls
    5  cd RuleTestFramework-main
    6  cd Tools
    7  cd calderaToAttire/
    8  ls
    9  cat README.md 
   10  git clone https://github.com/improsec/calderaToAttire
   11  ls
   12  cd calderaToAttire/
   13  ls
   14  cp /home/analyst/Downloads/EDR Test Simulation_report.json .
   15  cp /home/analyst/Downloads/EDR\ Test\ Simulation_report.json .
   16  python3 CalderaToAttire.py EDR\ Test\ Simulation_report.json
   17  ls
   18  sudo apt install -y debian-keyring debian-archive-keyring apt-transport-https curl
   19  curl -1sLf 'https://dl.cloudsmith.io/public/caddy/stable/gpg.key' | sudo gpg --dearmor -o /usr/share/keyrings/caddy-stable-archive-keyring.gpg
   20  curl -1sLf 'https://dl.cloudsmith.io/public/caddy/stable/debian.deb.txt' | sudo tee /etc/apt/sources.list.d/caddy-stable.list
   21  udo apt update
   22  sudo apt update
   23  sudo apt install caddy
   24  sudo apt-get update
   25  sudo apt-get install ca-certificates curl
   26  sudo install -m 0755 -d /etc/apt/keyrings
   27  sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
   28  sudo chmod a+r /etc/apt/keyrings/docker.asc
   29  echo   "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" |   sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
   30  sudo apt-get update
   31  sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin -y
   32  mkdir -p /opt/vectr/cert
   33  cd /opt/vectr/cert
   34  openssl genrsa -out ca.key 2048
   35  openssl req -x509 -new -nodes -key ca.key -sha256 -days 3650 -out ca.pem
   36  openssl genrsa -out server.key 2048
   37  openssl req -new -key server.key -out server.csr
   38  openssl x509 -req -in server.csr -CA ca.pem -CAkey ca.key -CAcreateserial -out server.crt -days 365 -sha256
   39  openssl x509 -in server.crt -text -noout
   40  cd /opt/vectr
   41  wget https://github.com/SecurityRiskAdvisors/VECTR/releases/download/ce-9.3.3/sra-vectr-runtime-9.3.3-ce.zip 
   42  unzip sra-vectr-runtime-9.3.3-ce.zip
   43  nano /etc/hosts
   44  ls
   45  unzip ra-vectr-runtime-9.3.3-ce.zip
   46  wget https://github.com/SecurityRiskAdvisors/VECTR/releases/download/ce-9.3.3/sra-vectr-runtime-9.3.3-ce.zip 
   47  unzip sra-vectr-runtime-9.3.3-ce.zip
   48  ls
   49  ls -la
   50  nano .env
   75  sudo docker compose up -d
