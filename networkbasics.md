OSI model is theoritical framework By iso 
#topic one osi model ( open source interconnection model ) it is developed as a way to help disparate computing systems communicate with each other.
There is total seven layers in osi model 
 layer -1 physical layer
 layer -2 data link layer
 layer -3 Network
 layer -4 Transport
 layer -5 Sessions
 layer -6 Presentation
 layer -7 Application


 >>layer -1 devices >> modem , hub 
 -analog modem ( modulation and demodulation)
 take the analog signal from the wire and convert it into digital signal that node could understand that is demodulation 
 take the digital signal from the node and convert it into an analog signal to be placed on the wire 
 ..They provides a single connection to the network.

HUBS? 
a hub function as a concentrator/ repeator in that it doesn't care where the signal comes form or where it is going 
it takes the electrical signal that arrives on a port and replicates that signal out all of the other ports . 
Ahub may have just few port or many ports
Not common in modern Networking


>>Layer-2 devies >> Switch , WAP

switch utilizes an application specific integrated circuit ( asic) chip 
the asic chip has specific programming that allow the switch to learn when a device is on the network and which ports it  is connected to via that device's layer 2 Mac address
switch - a smart hub 
can be simple and highly complex and programmable 
only commmunicates with the local network devices


WAP ( wireless acess point ) 
A wap  is a specific type of network bridge that connects (bridges) wirelss networks segments with wired network segments
only communicate with local network devices


>>Layer-3 MLS(multi layer switch), router
Mls(multi layer switch)- provides a normal layer2 network switching services but it will also provide layer3 or higher osi model serives 
the most commmon MLS is a layer3 switch 
it ony utilize an Ascii chip for switching but that asic chip also programmed to handle routing functions.this allows the devices to communicate and pass to non local network devices
they are highly programmed and complex in nature
just have few ports, may have many ports.


ROUTER?
A router is the most common network device for connecting different networks together utilizing the osi layer3 logical network information . 
the router uses software programming for decision making as compared to the switch use of an ASIC chip 
> the router uses this programming to keep track of differnet network and what if consider to be the best possible route to reach those networks 
> A router can communicate with both local and non local network devices .


>>Security devices : firewall > can be both physical device and software depending upon your needs. 
>software firewall, cloud firewall, hardware firewall
A firewall can be placed on routers and hosts (software based) or can be its own device. 
it functions at multiple layer of the osi model specifically at layer 2,3,4 and 7
it blocks packet from entering or leaving the network.
>>via stateless inspection : the firewall will examine every packet against a set of rules. ONce the packet matches a rule, the rule is enforced, and the specified action is taken.
>>via statefull inspection : the firewall will only examine the state of the connection between networks Spcifically when a connection is made form an inernal network to an external connection. As a general rule. external connections are not allowed to be initiated with the internal network
it is the first line of defense to protect internal network from outside threats

>>Security devices : instrusion detection system ( ids)
an ids is a passive system designed to identify when a network breach or attack against the network is occuring 
usually designed to inform a network administrator when a breach or attack has occured through log files , sms , and or an email notification. 
An Ids can't prevent or stop the breach or attacks. 
it recieve the copy of all traffic and evalaute it against a set of standards. 
>Signature based : evaluates network traffic for known malware or attack signatures. 
> Anomaly basesd : evaluates network traffic for suspicious changes. 
> Policy based : evaluates network traffic against a specific declared security policy. 
May be deployed at the host level : host based instrusion detection system(HIDS)

>>Security devices > IPS(instrusion prevention system)
an IPS  is an active system designed to stop a breach or attack from succeeding in damaging the network. 
Usually designed to perform an action or set of action to stop the malicious activity. 
Will inform a netwrok adminstrator through the use of log file , sms or email notification. 
All traffic on the network segment flows through the IPS to either enter or leave the segment. 
Like the ids , all the traffic is evaluated against a set of standards
the best placement on the network is between a routher ( with a firewall) and the destination network segment
It is programmed to make an active response to the situation
>blocking the offending ip address.
> close down the vulnerable interface. 
> terminate the network sessions
> redirect the attack  and much more 