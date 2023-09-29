# Joining-The-Client-To-The-Domain

<p align="center">

</p>

<h1>Active Directory - Joining The Client To The Doamin</h1>
This tutorial outlines joining the client to the domain using virtual machines in Microsoft Azure.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Client-1 virtual machine
- DC-1 virtual machine

*On the Azure portal go to the client-1 virtual machine and select the network interface* 

![Changing Client 1's Network Interface (1)](https://github.com/Ken7281/Joining-The-Client-To-The-Domain/assets/142465932/9fd24460-4903-4c72-bacb-a279fa9aae12)

*Doubleclick on the DNS servers and select the custom bubble and enter the private ip adress for DC-1 and click save* 

![Changing Client 1's Network Interface (2)](https://github.com/Ken7281/Joining-The-Client-To-The-Domain/assets/142465932/15dc569b-6f64-4f9e-9ec0-c01ec6fbe74f)

*Once the client-1 virtual machine is done updating restart it*

*Remote desktop back into Client-1 and go to the sysyem settings*
*Under the about section select rename this PC and select change*
*Click on the Domain bubble and type in mydomain.com and click ok*

![Linking Client 1 To Mydomain com](https://github.com/Ken7281/Joining-The-Client-To-The-Domain/assets/142465932/833354ae-17fb-4d5e-bfcd-8c2960d0472c)

*Enter the name of the previously created user and enter the password*
*You will get a message that says welcome to mydomain.com and the client-1 will need to restart*
*The client-1 virtual machine is now connected to the domain DC-1*
