# AWS-Solution-Architecture

<h2> Amazon Web Services: EC2 Instances </h2>
![image](https://github.com/Vaibhavsp/AWS-Solution-Architecture/assets/100761402/23349df7-a1f9-4160-8a37-eb1764d2fc71)
  
<h3>1. Run an EC2 instance in SSH</h3>

- <h5>Command to run EC2 Instance in SSH:</h5>

> Command:<br>
> ssh **"Public IPV4 Address"** -l **"Username"** -i **"Key_Pair_Name"**
> 
> Example:<br>
> ssh **"192.168.1.2"** -l **"ec2-user"** -i **"aws_key.pem"**
<br>


<h3>2. AWS SSH Socks5 Proxy</h3>


- <h5>Command to run EC2 Instance in SSH for **Socks5 Proxy**:</h5>

> Command:<br>
> ssh **"Public_IPV4_Address"** -l **"Username"** -i **"Key_Pair_Name"** -N -D **"Port_Number"**
>
> Example:<br>
> ssh **"192.168.1.2"** -l **"ec2-user"** -i **"aws_key.pem"** -N -D **"9090"**
