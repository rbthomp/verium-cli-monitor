Verium CLI Monitoring
=====================
This is a no client version of https://github.com/bezeredi/verium-cli-monitor
All credit for the display code goes to bezeredi.

![alt text](https://github.com/bezeredi/verium-cli-monitor/blob/master/cli-monitor.png "CLI Monitor Preview")


### How To Install & Use
This monitor currently supports `cpuminer` API version 1.1. This means that it
should work with the following CPU miners:
 * [Fireworm71's veriumMiner](https://github.com/fireworm71/veriumMiner)
 * [effectsToCause's veriumMiner](https://github.com/fireworm71/veriumMiner)
 * [tpruvot's cpuminer-multi](https://github.com/tpruvot/cpuminer-multi)


```python
#! monitor.py
port = 4048   #! NOTE: Change port numbers to those in use by your miners
```


1) Install `python3`, `pip3`
```bash
sudo apt-get install python3 python3-pip
```

2) Copy `monitor.py` to a machine on your LAN that can reach all of your mining
machines (for me, that was on my LAN controller). Create a file called
`.chosts` in your user's home directory and add the IP of each mining machine
on your LAN (hostnames can be used if you are running DNS or have them
enumerated in your `/etc/hosts` file)

5) Run `./monitor.py` and you should see statistics coming from each of your
mining machines


### Monitor Controls
 * Arrow Up, Arrow Down - Up and down
 * Home, End - First worker, last worker
 * q, ESC - Quit

### License & Donations
Free to use, just give credit where it's due. If this software helped you out,
consider a small donation.

VRM: VBwPRc7gmmqgJTsiB6LqsStVk2nxgRoyjh
