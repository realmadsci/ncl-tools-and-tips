# Wireshark

[Wireshark](https://www.wireshark.org/download.html) is the free tool of choice for this section.
You can typically use the "Portable Apps" version because you won't need to actually capture traffic.
That is often more convenient because it doesn't need any special priviledge to install and can be removed easily.

For DNS, look for packets with the DNS protocol or "Standard Query" in the info section
Afterwards, check for the packet with "Standard Query Response"

When dealing with HTTP, try looking for requests or http.response

If trying to check info about the files transferred, export the objects

When looking at TelNet, follow the TCP stream

For filtering out known protocols such as TCP and HTTP, use this filter: tcp && !(tcp.port == 22) && !(tcp.port == 80)

To find IVs use this filter: wlan.wep.iv
    After this, look for the WEP parameters. The IV is the initialization vector

To find the TCP checksum of a PCAP file:
    Use the previously acquired WEP key to decrypt traffic in Wireshark.
    Select "Edit > Preferences > Protocols > IEEE 802.11"
    then checking "Enable decryption" and adding the decryption key

A deauth attack may use this filter: wlan.fc.type_subtype  eq 12