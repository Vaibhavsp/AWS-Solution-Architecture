# AWS-Solution-Architecture

<h2> Amazon Web Services: EC2 Instances </h2>
  
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

After running this command:
> 1. Open new terminal of windows
> 2. Paste this in that rerminal:
> 
> "C:\Program Files\Google\Chrome\Application\chrome.exe" --user-data-dir="%USERPROFILE%\proxy-profile" --proxy-server="socks5://localhost:9090"
> Note: First check whether you chrome browser is stored. In my case Google Chrome is stored in **"Program Files"** in your case it should be in **"Program Files (x86)"**
