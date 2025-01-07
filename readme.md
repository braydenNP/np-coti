hello

# 1 Install Wazuh

sudo apt install curl

```bash
curl -sO https://packages.wazuh.com/4.9/wazuh-install.sh && sudo bash ./wazuh-install.sh -a
```

Go to https://127.0.0.1:443 in web browser

Login with provided username and password
```
admin
eqc*ztscrL.I5fICce4GU4k*7Q?YE7TL
```



# 2 Install Agent


amd64
```bash
wget https://packages.wazuh.com/4.x/apt/pool/main/w/wazuh-agent/wazuh-agent_4.9.2-1_amd64.deb && sudo WAZUH_MANAGER='192.168.8.103' WAZUH_AGENT_GROUP='default' WAZUH_AGENT_NAME='client' dpkg -i ./wazuh-agent_4.9.2-1_amd64.deb

sudo systemctl daemon-reload
sudo systemctl enable wazuh-agent
sudo systemctl start wazuh-agent

```

