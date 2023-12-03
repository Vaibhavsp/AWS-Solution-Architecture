# AWS-Solution-Architecture


<h3>###Run an **EC2 instance** in **SSH**</h3>
<br>

#####Command to run EC2 Instance in SSH:
ssh **Public_IPV4_Address** -l **Username** -i **Key_Pair_Name**
<br>
<br>
<br>

###AWS **SSH Socks5 Proxy**
<br>

#####Command to run EC2 Instance in SSH for **Socks5 Proxy**:
ssh **Public_IPV4_Address** -l **Username** -i **Key_Pair_Name** -N -D **Port_Number**

Example:
ssh **192.168.1.2** -l **ec2-user** -i **aws_key.pem** -N -D **9090**
