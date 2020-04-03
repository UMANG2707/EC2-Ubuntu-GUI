# EC2-Ubuntu-GUI
With using amazon free account create ec2 ubuntu instance and access it's GUI using remote desktop.

###  3 Steps to connect to the instance.

1. Configure Free Tier Ubuntu instance on AWS EC2
2. Connect to Ubuntu instance via SSH with PuTTY
3. Add GUI options to Ubuntu
4. Configure PuTTY to Tunnel RDP traffic
5. Test with RDP

### Step 1 Configure Free Tier Ubuntu instance on AWS EC2

- Login to AWS Educate Account.
- Go to the services and click on EC2.

<img width="960" alt="2020-04-03 (32)" src="https://user-images.githubusercontent.com/48994342/78326240-8760c900-7597-11ea-9b01-c4ea8475420e.png">

- Click on launch Instance.

<img width="960" alt="2020-04-03 (1)" src="https://user-images.githubusercontent.com/48994342/78326131-305af400-7597-11ea-955e-8b27a8fd1004.png">

- Select an Amazone Machine Image as Ubuntu Server 16.04.

<img width="960" alt="2020-04-03 (2)" src="https://user-images.githubusercontent.com/48994342/78326647-87ad9400-7598-11ea-8e6b-1c1792efb282.png">

- Choose an instance type t2.micro (Which is free).

<img width="960" alt="2020-04-03 (3)" src="https://user-images.githubusercontent.com/48994342/78326662-91cf9280-7598-11ea-9faa-dbc3b683ab6f.png">

- Click on Launch.

<img width="960" alt="2020-04-03 (4)" src="https://user-images.githubusercontent.com/48994342/78326672-97c57380-7598-11ea-9f41-76d26ceac3fa.png">

- Create key pair value if you already have you can choose that exist key pair.
- Give Key Pair Name.
- Download that key pair file (Key pair name + .pen).

<img width="960" alt="2020-04-03 (5)" src="https://user-images.githubusercontent.com/48994342/78326681-9e53eb00-7598-11ea-954b-c764a1515816.png">

- Click on Lounch Instance.

<img width="960" alt="2020-04-03 (7)" src="https://user-images.githubusercontent.com/48994342/78326692-a3b13580-7598-11ea-8ca6-16afcbb3dee6.png">

- Instance is Launched.
- Now, Click on View Instances.


<img width="960" alt="2020-04-03 (9)" src="https://user-images.githubusercontent.com/48994342/78326702-a7dd5300-7598-11ea-83c6-310169c18353.png">

- You can edit the name of instances.

<img width="960" alt="2020-04-03 (10)" src="https://user-images.githubusercontent.com/48994342/78327751-4074d280-759b-11ea-9fcb-dbbbd8bb1274.png">

- For edit the name of instance click on pen sign which is in Name column.

### step 2 Connect to Ubuntu instance via SSH with PuTTY
.
- For Download PuTTY open link given below.

 ##### https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html
 
 <img width="890" alt="2020-04-03 (11)" src="https://user-images.githubusercontent.com/48994342/78327753-41a5ff80-759b-11ea-9f5f-a41cd2c04db1.png">

- Now, Download PuTTY installer.
- After that install PuTTY.

- Open PuTTYgen.

<img width="515" alt="2020-04-03 (12)" src="https://user-images.githubusercontent.com/48994342/78327759-42d72c80-759b-11ea-87c0-8bb80c70f680.png">

- Load Keypair file which we have download.(keypair.pen)

<img width="365" alt="2020-04-03 (13)" src="https://user-images.githubusercontent.com/48994342/78327769-466ab380-759b-11ea-8c04-7d638f29aced.png">

- Select key Pair Name file which we have downloaded during step 1 process.(.pen File)

<img width="455" alt="2020-04-03 (14)" src="https://user-images.githubusercontent.com/48994342/78327773-48cd0d80-759b-11ea-8c7d-0dead6180316.png">

- It will show you only private key (.ppk) files for selecting .pen file select All Files *.

<img width="461" alt="2020-04-03 (15)" src="https://user-images.githubusercontent.com/48994342/78327792-51254880-759b-11ea-8fbe-4ed3d449306b.png">

- Save Private key (.ppk file).'

<img width="346" alt="2020-04-03 (17)" src="https://user-images.githubusercontent.com/48994342/78327804-55516600-759b-11ea-97c1-32ed4cdb5082.png">

<img width="450" alt="2020-04-03 (18)" src="https://user-images.githubusercontent.com/48994342/78327807-56829300-759b-11ea-88f9-3b44fa1bd5ed.png">

### step 4 Connect to the instance.
- Open PuTTY.

<img width="572" alt="2020-04-03 (19)" src="https://user-images.githubusercontent.com/48994342/78327810-58e4ed00-759b-11ea-94d3-f217dc8be7b3.png">

- Select public IPV4 of instance.

<img width="813" alt="2020-04-03 (20)" src="https://user-images.githubusercontent.com/48994342/78327825-5c787400-759b-11ea-961c-d135c7d00d29.png">

- Give that ip as host.

<img width="331" alt="2020-04-03 (21)" src="https://user-images.githubusercontent.com/48994342/78329063-5932b780-759e-11ea-9d2b-0bd09aa88ef1.png">

- Save this session data to any session variable.

<img width="325" alt="2020-04-03 (22)" src="https://user-images.githubusercontent.com/48994342/78329066-5afc7b00-759e-11ea-8bdc-5fe022f7e06a.png">

- Click on Connection -> SSH -> Auth.

<img width="328" alt="2020-04-03 (25)" src="https://user-images.githubusercontent.com/48994342/78329071-5d5ed500-759e-11ea-81d5-42530fc51303.png">

- Browse that private key file which we have generated using PuTTYgen.
- Click on Open.

<img width="335" alt="2020-04-03 (26)" src="https://user-images.githubusercontent.com/48994342/78329122-7f585780-759e-11ea-9478-6288294ba67a.png">

- Can Use access instance CLI.

<img width="530" alt="2020-04-03 (28)" src="https://user-images.githubusercontent.com/48994342/78329138-854e3880-759e-11ea-9610-85cf71d69e92.png">


### step 3 Add GUI options to Ubuntu

- Followe given Comands to add GUI option in ubuntu.

- Check For update and install upgrads run follwing command.
  > sudo apt update &&  sudo apt upgrade
  
- We will connecting using windows remote desktop, edit the ssds_config file in your linux instance for allowing password authantication.
  > sudo sed -i 's/^PasswordAuthentication no/PasswordAuthentication yes/' /etc/ssh/sshd_config

- Restart SSH daemon to make this change.
  > sudo /etc/init.d/ssh restart

- To gain root privileges and set password for ubuntu user for security.
  > sudo passwd ubuntu

- Install xrdp tool for desktop environment (Virtual Network Computer).
  > sudo apt install xrdp xfce4 xfce4-goodies tightvncserver

- Make xfce4 default window manager for Remote Desktop Connection.
  > echo xfce4-session$ /home/ubuntu/.xsession  ##### NOTE: Replace the $ with the Greater Than Sign

- Copy .xsession to the /etc/skel folder so xfce4 is set as default window manager for any new user account.
  > sudo cp /home/ubuntu/.xsession /etc/skel

- Run sed command to allow changing of the host port you will connect to.
  > sudo sed -i '0,/-1/s//ask-1/' /etc/xrdp/xrdp.ini

- Restar xrdp service.
  > sudo service xrdp restart
  
- Now, exit from the instance.
  > exit

### step 4 Configure PuTTY to Tunnel RDP traffic

- Open PuTTY.
- Load Session in which we saved information.
  [ If you have not saved session information then you have to put host name and browse that private key file again ]
- Now, Go to Connections -> SSH -> Auth -> Tunnels.
- Give Source port as 8888 and in Destination field give private IPV4 of your instace with addition of : and another port as 3389.
- Click on open.
- Login as ubuntu [If your instance's AMI is ubuntu]
- For checking port is working or not follow given command.
 > netstat -antp
 - Remember IPV4 which is in resukt of above command and source port address.
 
### step 5 Test with RDP

- Start Remote Desktop from your Windows Operating System.
- Give IPV4 and source port with (:) seperated and connect.
- you can use EC2 instance with GUI.
- Now, Give Username as ubuntu and password which you had set for root privileges.


