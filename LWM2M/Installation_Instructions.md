I have installed Leshan by following professor’s instructions. Initially I had trouble setting up my router. I couldn’t connect to VUMobile or VUGuest. So, I 
connected to the ethernet provided by professor.
First I logged on to the Raspberry Pi by using the command “ssh dietpi@IPADDR” (IPADDR is the IP address of Diet Pi) and then by typing in the password.
Later I installed git by typing in the command “sudo dietpi-software” . Then I searched for the software git and installed it. I have checked the version of git by
using the command “git –version”.
In the next step, I have installed java jdk by using the command “sudo dietpi-software” and by searching for jdk. It took a while for installation. Later I have checked
that it was installed by using the command “java - -version”.
Further, I have created a directory called “download“ in the dietpi. Changed to the download directory by using the cd command and then downloaded the latest version of
maven using wget.
Next, I have setup environment variables to add to maven paths and then confirmed the maven installation.Later I have installed leshan git and then built it. The 
process took a bit of time.Next I started the leshan server and then connected on to leshan demo by using the command UI: http://RPI_IPADDR:8080 
(where RPI_IPADDR is the pi’s IP address). Lastly, I have used the command
" java -jar leshan-client-demo/target/leshan-client-demo-*-SNAPSHOT-jar-with-dependencies.jar " in the command prompt, which added the dietpi to the leshan page.
![image](




