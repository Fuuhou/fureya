# UPDATE VPS
<pre><code>sysctl -w net.ipv6.conf.all.disable_ipv6=1 >/dev/null 2>&1 && sysctl -w net.ipv6.conf.default.disable_ipv6=1  >/dev/null 2>&1 && apt update -y && apt upgrade -y && apt install xz-utils screen -y</code></pre>

# INSTALL SCRIPT 
<pre><code>wget https://raw.githubusercontent.com/Fuuhou/fureya/main/main.sh && chmod +x main.sh && sed -i -e 's/\r$//' main.sh && screen -S main ./main.sh</code></pre>

# UPDATE MENU
<pre><code>wget https://raw.githubusercontent.com/Fuuhou/fureya/main/update.sh && chmod +x update.sh && sed -i -e 's/\r$//' update.sh && screen -S update ./update.sh</code></pre>

# OS SUPPORT
- DEBIAN 10 , 11
- UBUNTU 18 , 20
