# aircrack-ng

A Docker image containing Aircrack is available in [Docker Hub](https://hub.docker.com/r/realmadsci/aircrack-ng) so it can
be quickly used by simply running `docker run --rm -it --volume $env:USERPROFILE/Documents:/host realmadsci/aircrack-ng` (for mounting your Documents folder as `/host/` when starting this from Powershell).
It is also fairly easy to install on Kali (`sudo apt install aircrack-ng`).

The aircrack tool can be used for wireless password cracking, such as pcap files with WEP encryption.
To run aircrack, simply use the following command: aircrack-ng <file_name>
    or, if you need to use a wordlist: aircrack-ng -w <wordlist> -b <mac_addr> <file_name> 

    key size = (bytes in key * 8 bits) + IV
    (typically IV is 24 bits; If this is wrong, then look up WEP key sizes and find one that the bits in the key match closest)

WEP parameters can be found in the IEEE section of Wireshark while a packet is selected.

To add a WEP key for decryption go to:“Edit > Preferences > Protocols > IEEE 802.11" and then check "Enable decryption" and add the key.

TCP checksums can be found in the Transmission Control Protocol section in Wireshark while a packet is selected.