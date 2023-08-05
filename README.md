<p align="center">
<img src="https://github.com/niloymridul/vpntalked/assets/139414980/16ae9092-7716-4654-ae1b-1e0f011b7819" height="40%" width="40%" alt="Kali Linux logo"/>
</p>

<h1> Virtual Private Networks Explained and Shown</h1>
Welcome to the VPN tutorial. This part of the tutorial will be explaining the usage of VPN's and how to use them for real life purposes.<br />

<h2>Environments & Softwares Used</h2>

- Microsoft Azure
- Virtual Machines
- ProtonVPN 
  
<h2>Project Steps</h2>

<p>
VPN Tutorial

Welcome to the Virtual Private Network tutorial. Here we are going to talk about VPN's and what they do. But before we talk about VPN's we need to start with the basics. What is a modem and a router?

When it comes to tech like these, most people just have it installed via there internet service provided(Verizon, Spectrum and any other company that provides internet services). A modem is the box that connects your home network to your internet service provide. A router is the box that connects all your wireless and wired devices together. A home network is all the devices connected to your router at your own home work place. A Hotspot(which public networks often use) are business class routers/hardware set up throughout the area so that anyone can connect to it. 

Now, Virtual Private Networks are (as the title says) a private network. These are established when you download the software and turn it on and connect to the location you wish to connect to(more on that later.) While there are home networks, there are also other forms. Some places have public networks you can access but there is a problem with them.

Because some locations are public that means any devices/anyone can connect to them. Let's say for example, you arrive in a Cafe and you need to send an email to your boss before a deadline that is coming up. You connect to the cafe's local network. Unlike your home/local network, cafe's use hotspots but they still have the same process of connecting everything into one network.

Let's say you try to connect to the local wifi. When you do, you see they are two wifi spots that have the same name but one's capitalized and the other isn't. You connect to one of them without giving a care and now all of a sudden, your computer is suddenly slow and crashing because all of it's ram and cpu being used entirely all of a sudden. 

Now this is just one out of many scenarios when getting attacked digitally after connecting to public wifi. When you use your home router and modem setup, no one else outside of the people you know and have permission can use the internet.  And with certain modem's and routers, you can even add certain controls such as password protection, website filtering, time restrictions and more. With public wifi such as cafe's, do not have these controls and you do not know who is connected. And with hotspots, they can also use tools to see other people's IP address and more information because they are connected to the internet and you share connections with everyone else.

VPN's help prevent forms of hacking happening as VPN can hide your IP address making it harder to detect your location. VPN's also encrypt's your data so that when you send data to do work it will prevent any one else from being able to unlock and see it. Note: Encryption is converting data into code that hides the data's actual information until it is decrypted. The only way to decrypt data is to have the password for it thus making it harder, if not, impossible to look at said data. 

A lot of ad's you see online today whether it be on the internet or on TV talk about how useful an ad is but a lot of the time, in order to use them you have to input your information and pay for them. For this tutorial, you will just need a temporary account to get some experience. While there are many VPN's to choose from, we will use ProtonVPN for now and we will test it out on a VM in Azure.

First thing we will do is check our IP address. While there are many ways to do it such as typing command in the console, we can use this website instead. Click on this first to see your IP Address. We are going to keep this in mind and compare it to the othertimes we check for it.

--ip address website 1st--

[Click here to see your IP Address!](https://whatismyipaddress.com/)

--azure vms--

With this in mind, we are now going to create a Virtual Machine in Azure. First, log in to your Azure account. Make one if you haven't done it. When you hit create we are going to fill out some information. 

--create vm--

We will have to create a Resource Group first. You can name it whatever you want, just make sure one is created so that we can ensure that our VM can have all it's information stored somewhere. Name it whatever you want as well so long as it is remembered. Region should be whatever it is you want so in this case I will make it Canada Central so that VM's IP Address will be different then the one we checked beforehand. 

--vm image--

We will then have to choose an image for the Virtual Machine. What this means is that we need to choose the OS aka Operating System for the VM. Furthermore, we will also need to make an Username and Password for this account. Make it whatever you want but write it down and remember it. For size we will use 4 CPU's with 16 gigabites. We do not need to lower the settings but if you want to go ahead. We will only use this briefly if anything. Then click on the checkbox in Licensing and hit create. If it doesn't create immediately then try again in a few seconds and then if not then double check your work and or click on the area and then hit review and create.

--New VM--

Wait a few seconds for it to finish deploying and then we will have to connect to it. Once enough time has passed, go to the home page on Azure then click Virtual Machines then the VM you named and creating. I want you to connect to the VM whatever method your OS system is via RDP aka Remote Desktop Protocol. Copy the IP address that the VM has and connect it.

--log in rdp--

When log in via RDP, you will have to click on more choices, and then log in via the credentials we set up earlier. Now go ahead login. Click yes for certificates pop up and say no to all Privacy Settings. Click on Microsoft Edge and then go to the same website as before. Write/keep in mind the current IP Address and compare it to the previous IP Address we checked before.

--protonvpn free & clients--

We will then download ProtonVPN. Go to the ProtonVPN website, download and look down to click and download protonVPN free. Create an account to download ProtonVPN and then install it. Because we are using a Windows Computer we will install it via Windows. For installing it, click install and click next. 

--quick connect--

After installing it, it should open. Log in with your credentials and then familiarize yourself with the interface. You do not need to take a tour if you don't need to. If anything just do quick connect or choose the location yourself. Even addresses in other continents. Then go back to the website and double check the IP Address. Now compare all the ip addresses you've had seen all these times. 

--Google netherlands--

One more interesting thing about this is that because of this change in IP and location it also affects how websites perceive you. Because my IP address was in the Netherlands due to ProtonVPN, Google sends me this message. This also applies to other websites too. Experiment with it.

Now the last thing you should to save money is to delete all resources used. In this case, it becomes easier as all you have to do is just simply delete the resource group holding the VM so it deletes everything. You will also need to delete NetworkWatcherRG as whenever you create a VM on Azure this NetworkWatcherRG will be created typically.

Now you know how exactly VPN's work, what they do and how useful they are. Hopefully, you will start using them now to the best of your ability and stay safe in this digital age.
