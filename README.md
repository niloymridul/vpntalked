<p align="center">
<img src="https://github.com/niloymridul/vpntalked/assets/139414980/16ae9092-7716-4654-ae1b-1e0f011b7819" height="40%" width="40%" alt="Kali Linux logo"/>
</p>

<h1> Virtual Private Networks Explained and Shown</h1>
Welcome to the VPN tutorial. This part of the tutorial will be explaining the usage of VPN's and how to use them for real-life purposes.<br />

<h2>Environments & Softwares Used</h2>

- Microsoft Azure
- Virtual Machines
- ProtonVPN 
  
<h2>Project Steps</h2>

<p>
VPN Tutorial

Welcome to the Virtual Private Network tutorial. Here we are going to talk about VPN's and what they do. But before we talk about VPN's we need to start with the basics. What is a modem and a router?

When it comes to tech like this, most people just have it installed via their internet service provided(Verizon, Spectrum, and any other company that provides internet services). A modem is a box that connects your home network to your internet service provider. A router is a box that connects all your wireless and wired devices together. A home network is all the devices connected to your router at your own home workplace. A Hotspot(which public networks often use) are business-class routers/hardware set up throughout the area so that anyone can connect to it. 

Now, Virtual Private Networks are (as the title says) private networks. These are established when you download the software and turn it on and connect to the location you wish to connect to(more on that later.) While there are home networks, there are also other forms. Some places have public networks you can access but there is a problem with them.

Because some locations are public that means any devices/anyone can connect to them. Let's say, for example, you arrive at a Cafe and you need to send an email to your boss before a deadline that is coming up. You connect to the cafe's local network. Unlike your home/local network, cafes use hotspots but they still have the same process of connecting everything into one network.

Let's say you try to connect to the local wifi. When you do, you see they are two wifi spots that have the same name but one's capitalized and the other isn't. You connect to one of them without giving a care and now all of a sudden, your computer is suddenly slow and crashing because all of its ram and CPU are being used entirely all of a sudden. 

Now this is just one out of many scenarios when getting attacked digitally after connecting to public wifi. When you use your home router and modem setup, no one else outside of the people you know and have permission can use the internet.  And with certain modems and routers, you can even add certain controls such as password protection, website filtering, time restrictions, and more. With public wifi such as cafes, do not have these controls and you do not know who is connected. And with hotspots, they can also use tools to see other people's IP addresses and more information because they are connected to the internet and you share connections with everyone else.

VPNs help prevent forms of hacking happening as VPNs can hide your IP address making it harder to detect your location. VPNs also encrypts your data so that when you send data to do work it will prevent anyone else from being able to unlock and see it. Note: Encryption is converting data into code that hides the data's actual information until it is decrypted. The only way to decrypt data is to have the password for it thus making it harder, if not, impossible to look at said data. 

A lot of ads you see online today whether it be on the internet or on TV talk about how useful an ad is but a lot of the time, in order to use them you have to input your information and pay for them. For this tutorial, you will just need a temporary account to get some experience. While there are many VPNs to choose from, we will use ProtonVPN for now and we will test it out on a VM in Azure.

The first thing we will do is check our IP address. While there are many ways to do it such as typing commands in the console, we can use this website instead. Click on this first to see your IP Address. We are going to keep this in mind and compare it to the other times we check for it.


<p align="center">
<img src="https://github.com/niloymridul/vpntalked/assets/139414980/082e24bf-a9f6-40a8-98cb-a2823d05d0c2" height="70%" width="70%" alt="IP Address"/>
</p>

[Click here to see your IP Address!](https://whatismyipaddress.com/)

<p align="center">
<img src="https://github.com/niloymridul/vpntalked/assets/139414980/a5bb037d-55ef-4a51-a97a-1337041b956a" height="70%" width="70%" alt="Azure VM"/>
</p>

With this in mind, we are now going to create a Virtual Machine in Azure. First, log in to your Azure account. Make one if you haven't done it. When you hit create we are going to fill out some information. 

<p align="center">
<img src="https://github.com/niloymridul/vpntalked/assets/139414980/d6ea381e-2398-4980-b555-3a0ae244d409)" height="70%" width="70%" alt="Create Azure VM"/>
</p>

We will have to create a Resource Group first. You can name it whatever you want, just make sure one is created so that we can ensure that our VM can have all its information stored somewhere. Name it whatever you want as well so long as it is remembered. The region should be whatever it is you want so in this case I will make it Canada Central so that the VM's IP Address will be different than the one we checked beforehand. 

<p align="center">
<img src="https://github.com/niloymridul/vpntalked/assets/139414980/bf1c09f3-0dfa-4c3a-a17c-d93d7892bd38" height="70%" width="70%" alt="Image VM"/>
</p>

We will then have to choose an image for the Virtual Machine. What this means is that we need to choose the OS aka Operating System for the VM. Furthermore, we will also need to make a Username and Password for this account. Make it whatever you want but write it down and remember it. For size, we will use 4 CPUs with 16 gigabytes. We do not need to lower the settings but if you want to go ahead. We will only use this briefly if anything. Then click on the checkbox in Licensing and hit Create. If it doesn't create immediately then try again in a few seconds and then if not then double check your work and or click on the area and then hit review and create.

<p align="center">
<img src="https://github.com/niloymridul/vpntalked/assets/139414980/a840d707-bea6-458c-890c-46567c1739e4" height="100%" width="100%" alt="New VM"/>
</p>

Wait a few seconds for it to finish deploying and then we will have to connect to it. Once enough time has passed, go to the home page on Azure then click Virtual Machines then the VM you named and created. I want you to connect to the VM whatever method your OS system is via RDP aka Remote Desktop Protocol. Copy the IP address that the VM has and connect it.

<p align="center">
<img src="https://github.com/niloymridul/vpntalked/assets/139414980/6b191e45-5935-4cb8-a1de-5eb8e4949d33" height="40%" width="40%" alt="RDP"/>
</p>

When logging in via RDP, you will have to click on more choices, and then log in via the credentials we set up earlier. Now go ahead log in. Click yes for certificates pop up and say no to all Privacy Settings. Click on Microsoft Edge and then go to the same website as before. Write/keep in mind the current IP Address and compare it to the previous IP Address we checked before.

<p align="center">
<img src="https://github.com/niloymridul/vpntalked/assets/139414980/8e2271b9-73f8-4b6b-8806-960b899c35ad" height="70%" width="70%" alt="PROTONDOWNLOAD"/>
</p>


<p align="center">
<img src="https://github.com/niloymridul/vpntalked/assets/139414980/899a8d07-d366-4cf7-902f-e037abd13706" height="70%" width="70%" alt="PROTONDOWNLOAD"/>
</p>

We will then download ProtonVPN. Go to the ProtonVPN website, download, and look down to click and download protonVPN free. Create an account to download ProtonVPN and then install it. Because we are using a Windows Computer we will install it via Windows. For installing it, click install and click next. 

<p align="center">
<img src="https://github.com/niloymridul/vpntalked/assets/139414980/a87a3f23-40ac-40ed-976f-f54c4c3c5d74" height="70%" width="70%" alt="Quick Connect"/>
</p>

After installing it, it should open. Log in with your credentials and then familiarize yourself with the interface. You do not need to take a tour if you don't need to. If anything just do quick connect or choose the location yourself. Even addresses in other continents. Then go back to the website and double-check the IP Address. Now compare all the IP addresses you've seen all these times. 


<p align="center">
<img src="https://github.com/niloymridul/vpntalked/assets/139414980/310de2ba-45ec-492a-b7fc-abc358b91551" height="70%" width="70%" alt="PROTONDOWNLOAD"/>
</p>

One more interesting thing about this is that because of this change in IP and location it also affects how websites perceive you. Because my IP address was in the Netherlands due to ProtonVPN, Google sends me this message. This also applies to other websites too. Experiment with it.

Now the last thing you should to save money is to delete all resources used. In this case, it becomes easier as all you have to do is just simply delete the resource group holding the VM so it deletes everything. You will also need to delete NetworkWatcherRG as whenever you create a VM on Azure this NetworkWatcherRG will be created typically.

Now you know how exactly VPN's work, what they do and how useful they are. Hopefully, you will start using them now to the best of your ability and stay safe in this digital age.
