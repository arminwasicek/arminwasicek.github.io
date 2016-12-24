---
title: 2015 Automotive Security Panorama
date: 2015-12-24
description:
categories: 
  - automotive 
  - security
image:
author_staff_member: armin
---

2015 has been an exciting year regarding automotive security. Many autosec incidents have been reported in media and thus raised public awareness for the field. Some of these incidents triggered big time events. It has been the first time that car makers were pointed out by name because of their vulnerable models. The first cyber security related callback action has happened in 2015. Exploits have been disclosed in mainstream security conferences such as Black Hat and Defcon and stirred up a discussion on ethical disclosure in automotive security.



# AutoSec incidents 2015

![Checkmate](/images/2015_autosec_events.png)

## Diagnostic Interface Penetration testing

The year started with a hack on an OBD dongle used by the Progressive insurance company. The use of OBD dongles is increasing as it can be used to retrofit older cars to the Connected Car age. The autosec researcher performing this hack said that this particular device “basically uses no security technologies whatsoever”. Most likely, this applies to other OBD dongles as well.

## Man-in-the-middle of a Connected Car

Next BMW cars were targeted by a  relay attack. A fake cellular station was used to intercept the connection between the ConnectedDrive and a mobile phone issuing commands, e.g., to unlock the doors. On that occasion BMW demonstrated its Over-the-Air (OTA) capabilities for the first time and responded with updating its fleet remotely. The patch included encrypting the vulnerable connection.

## Remote Controlling a Connected Car

After some silence, the automotive security world was hit by the report of two automotive security researchers remote controlling a Jeep Cherokee with a Wired reporter on board. They managed to intrude the vehicle through its Connect, a device to connect the vehicle to the internet. The device was reachable through its IP address and the researchers could inject some malware to invoke window lifts, braking, etc. This event caught big attention in the community and in public. It triggered a manufacturer’s first call-back action because of cyber security concerns.

## Intercepting the Connected Car

The Onstar hack in the same month requires a physical device, the ‘OwnStar’ to be planted somewhere underneath a car’s body. It then uses its wireless capabilities to trick a driver’s phone into connecting. When the driver logs into the Onstar RemoteLink app, the device reads the user’s credentials and transmits those to the attacker. Using the driver’s credential, the attacker has full access to the driver’s Onstar system and can do anything that a legitimate user can do. From that point the OwnStar box is not needed anymore and can be removed from the car.

## Automotive Penetration Testing and Patching

Tesla has been targeted several times this year. Besides its corporate bounty program, two automotive security incidents went public: First, Chinese researchers claimed to be able to open the doors during driving the car. On this incident, not many details are available. In the second effort, researchers did some long term testing of the attack surface. Using physical access through an Ethernet port, they were able to access the internal network. From there on, they could use their internet security skills to hack into the internally used WebKit web browser and the internally deployed Ubuntu Linux. Altogether six vulnerabilities were found and patched through Tesla’s OTA capabilities.

## Crypto cracking to Unlock Cars

Cracking the Megamos crypto chip has already happened in 2013, but this year the court order preventing the publication has expired in August. The Megamos chip is being deployed in immobilisers of many brands (Audi, Fiat, Honda, Volkswagen and Volvo). An immobilizer is an anti-theft device which prevents the engine of the vehicle from starting when the corresponding transponder (key) is not present. Exploiting this vulnerability exposes many vehicles to theft. The researchers were able to recover the 96-bit secret key by listening to the wireless communication of the transponder with the vehicle.

## Insider Attacks On Emissions Control Systems

The Volkswagen DieselGate is a classic example of an insider attack: Insiders misuses their privileges to trick their peers. In the #DieselGate, the Volkswagen misused the trust its customers and regulatory bodies put into the company to deliver vehicles according to their specification. Volkswagen’s cars were not able to deliver that. On the contrary, they implemented a ‘deceit device’ which actively concealed the emission rating during test conditions. Academic researchers uncovered the plot, bringing the entire Volkswagen group in turmoil.

## Hack to increase E-Vehicle Range

The second BMW automotive security incident this year targeted the i3 which is the company’s electric model. If equipped with a range-extender, it stores a gasoline in its tank. Due to legislative differences, in California a zero-emission vehicle is only allowed a 1.9-gallon fuel tank, whereas European owner might in 2.4 gallons. Some US i3 owners claim to have found a software hack to unlock the half gallon from the European model. Both types of cars origin from the same assembly line in Leipzig. It makes sense for the manufacturer to build a generic i3 and then fit it to the respective market by switching the software configuration. We can expect to see more of this type of attack in the future, when software is increasingly deployed to customize vehicles.

## State Trooper Vehicle Penetration Test

Virginia’s state police has been collaborated with researchers for a penetration test of their Impala Police Interceptors. The researchers could access the vehicle bus and read and write commands that trigger actuators in the vehicle.

## Airbag hack

Finally, researchers claimed to have performed a zero-day exploit to disable airbags on Audi And potentially other VolkswagenGroup vehicles. They hacked a diagnostic tool to get access to the vehicles functions. The increasing number of software tools that connect to vehicles open another, new door for attackers to get to the vehicle. Requiring a certain privileges to operate, diagnostic tools could be increasingly targeted as other attack surfaces are being locked down.

 

# Where is Automotive Security going?

We classify the attacks in three classes:

* Penetration tests aiming to gauge the attack surface of certain cars
* Theft incidents that relate to the traditional car ownership patterns
* Circumventing legislation and cheating

Penetration tests have been the most public visible activity in the field so far. Stories of what attackers might be able to influence and gauging what are the effects on individuals receive interest of a broad audience listening to the media channels. This year’s successful penetration tests contributed to make the autosec field visible and raise the awareness to 'something needs to be done', even for those manufacturers that have not yet acted.

Theft protection is the traditional application (cyber-)security technologies in vehicles. Ever since the cars can use transponders to augment the capabilities of the mechanical key, cryptography, digital communication and handling of sensitive information has been an issue in vehicles. Still, getting a car in physical possession is one of the big motivations to attackers and automotive security researchers. As the traditional mobility patterns are changing, ownership patterns are changing, too. For instance, car sharing removes the necessity to maintain a vehicle for individuals and makes mobility even more affordable through resource pooling.

The last category might indicate where the field is going to. As it is software that effects the differentiation between products, we might see more such attacks in the future. Using a hack on one’s car to get a better service is something that even good people might eventually do. Like jailbreaking a smartphone is a widespread phenomena and not restricted to a conspirative subgroup. People might even be willing to pay for such exploits.

# Wrapping up AutoSec 2015

The year 2015 revealed that the car makers are at different stages implementing security countermeasures in their cars. Acknowledging that any car maker could be targeted by a successful attack, it is the recovery after the attack that makes a difference to the car holder. For instance, BMW and Tesla were able to quickly react to the reported attack vectors through their remote update functions. Jeep’s hack took more effort for remediation. The year’s autosec incidents not only showed the capabilities of different manufacturers, but also indicated where the field is going to. The automotive industry is becoming a service-oriented business and as such, it will have to deal increasingly with service-oriented hacks.