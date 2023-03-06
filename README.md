# DOT-vm
forensic machine designed to help analysts perform their job easily and efficiently

Dot VM is a forensic machine designed to help analysts perform their job easily and efficiently. It is a collection of open-source tools that includes Dissect, Log2timeline, Hayabusa, Timesketch, and ELK stack as a backend. 

Dot VM can handle many disk image formats directly, without the need for any additional tools or utilities. Here are some of the disk image formats that Dot VM can handle directly:

RAW disk image (.raw)
Split RAW disk image (.001, .002, .003, etc.)
VMware Virtual Disk Format (.vmdk)
Microsoft Virtual Hard Disk Format (.vhd, .vhdx)
EnCase Evidence File Format (.e01)

To use Dot VM and start analyzing disk images, follow these instructions:

- Open the Filebeat folder located on the desktop and execute the following command: ./filebeat -e -c monitor.yml.

- Open the Logstash folder and execute the following command: ./logstash -f /home/forensics/Desktop/logstash-8.6.2/Parssing.conf.

- To start the analysis, execute DOT.sh with the sudo command, it will provide the analyste with multipile choise to be selected , once the analysis done 
navigathe through the browser to 0.0.0.0:5601 to start discover the ingested data



To set up and run Timesketch, follow these instructions:

Navigate to the Timesketch directory by executing the following command: cd /opt/timesketch.

Start Timesketch with Docker by executing the following command: sudo docker-compose up -d.

After Timesketch is up and running, log in through Firefox to https://0.0.0.0 using the following credentials:

Username: forensics
Password: forensics

By following these instructions, you can effectively use Dot VM and Timesketch to perform forensic analysis on disk images.

Ref
-https://github.com/fox-it/dissect 
-https://github.com/log2timeline/plaso
-https://github.com/Yamato-Security/hayabusa
-https://www.elastic.co/elastic-stack/
-https://timesketch.org
