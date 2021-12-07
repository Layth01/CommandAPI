# IntrusionDetection Lab1 Snort
# Layth Chebbi 3 SSIR A

## 1. Installing SNORT on CentOS 8

![](1.png)

![](2.png)

![](3.png)

![](4.png)

![](5.png)

![](6.png)


## 2. Configuring SNORT to run as a NIDS

![](7.png)

![](8.png)

![](9.png)

![](10.png)

![](11.png)

![](12.png)

![](13.png)

## 3. Configuring the network and rule sets

![](14.png)

![](15.png)

![](16.png)

![](17.png)

![](18.png)

![](19.png)

## 4. Validating settings

![](20.png)

![](21.png)

![](22.png)

![](23.png)

![](24.png)

![](25.png)

![](26.png)

## 5. Adding our own rules to SNORT and generating alerts

![](27.png)

![](28.png)

![](29.png)

![](30.png)

![](31.png)

![](32.png)

![](33.png)

![](34.png)

### Detecting GIF file transfer

34.  Explain how to detect the existence of a GIF file inside a network traffic?

We can detect the existence of a GIF file using the signature of the GIF file as we did with png file.

35. Propose a snort signature allowing to detect GIF files transmitted over the network

```
alert tcp any any -> any any (content:"GIF89a"; msg:"GIF";sid:10000)
```
36. Which datagram(s) (inside the pcap file with_png.pcap) contain the transmitted GIF file ?

The datagram number 69 contains the transimited GIF file

![](35.png)

37. Test the new proposed snort rule and show the generated alert.

![](36.png)

![](37.png)

![](38.png)
