# systemd-pcap
for long running pcaps

Steps:
1. Place pcap-tool.service file in /etc/systemd/system/
2. chmod 644 /etc/systemd/system/pcap-tool.service
3. Customise settings such as pcap filter, file size etc in pcap-tool.service file
4. Start and stop using systemctl start|stop pcap-tool.service
