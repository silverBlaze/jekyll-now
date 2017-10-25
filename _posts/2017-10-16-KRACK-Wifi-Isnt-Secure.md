---
layout: post
title: "KRACK: Your WiFi Isn't Secure Anymore"
post_author: Jason Wells
---

![_config.yml]({{ site.baseurl }}/images/posts/2017-10-16-lock-header.jpg)

Early this Monday morning, a coordinated release will unveil a number of vulnerabilites in the WPA2 WiFi security protocol used on most wireless networks world-wide.

Currently being called the KRACK exploit (short for Key Reinstallation AttaCK,) the secretive proof-of-concept works by exploiting security handshakes that establish keys used for encrypting the WiFi network traffic.<!--more--> Other details are not yet known, but the research will be publicly disclosed on Monday at 8 AM, Eastern Time. Based on what we know now, the vulnerability likely exists during the four-way handshake, wherein the AP and client each prove they know the pre-shared key without disclosing it (see [Wikipedia](https://en.wikipedia.org/wiki/IEEE_802.11i-2004?lipi=urn%3Ali%3Apage%3Ad_flagship3_pulse_read%3BaJ3WwdNaSEWpDxopyTxbJg%3D%3D#The_four-way_handshake) for more on this part of the WPA2 protocol.)

## What does this mean?

It effectively means that you need to start treating your own WiFi network as if it was insecure. It is currently safe to assume that attackers will be able to eavesdrop on your wireless network traffic, and all indications are that such eavesdropping will be easy to pull off once the research goes live.

## What can you do?

You need to start behaving the same way you would if you were connected to an insecure hotspot at your local coffee shop. This means configuring the wireless connection or firewall settings as a "Public Network". On your mobile device, you can switch off WiFi and use your cellular data connection for greater security.

Remember, any web traffic going over HTTPS will still be encrypted with TLS/SSL, so you don't need to necessarily avoid online shopping and other web activity; just make sure you're taking normal precautions. You can even consider investing in a VPN service that can tunnel all of your device's traffic through an encrypted connection.

As for a long term fix, hopefully most router and hotspot manufacturers will start releasing updated firmware that can address these vulnerabilities. But there are no guarantees that such updates will be available soon (or at all.) Keep your eyes on the news and check with your manufacturer for when such an update might be released.

For more info, see this article:
[https://arstechnica.com/information-technology/2017/10/severe-flaw-in-wpa2-protocol-leaves-wi-fi-traffic-open-to-eavesdropping/](https://arstechnica.com/information-technology/2017/10/severe-flaw-in-wpa2-protocol-leaves-wi-fi-traffic-open-to-eavesdropping/)