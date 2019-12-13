# systemd-pcap
for long running pcaps

Steps:
1. Place pcap-tool.service file in /etc/systemd/system/
2. chmod 644 /etc/systemd/system/pcap-tool.service
3. Work out how much disk space you can safely use up for the captures
4. Customise settings such as pcap filter, file size etc in pcap-tool.service file
5. Start and stop using systemctl start|stop pcap-tool.service
6. Once the captures have started record the rate capture file sizes changes over 2 test interval periods and work out how many days of captures will be possible with the current pcap-tool configuration settings. You may be able to adjust snap length to get more days out when there are disk space limitations or captures need to run over several days or weeks.
