# GSoC 19 POW BitTorrent Client (1):

A BitTorrent Client to create, seed and download from .torrent files. Coupled with Data Integrity and Authenticity checks!

## Getting Started

This will guide you through setting up this BitTorrent client, this repository is split into 2 parts:

#### 1) Uploading:
This involves generating the Message Digest for Data integrity, creating .torrents and seeding the contents to other BitTorrent peers.

#### 2) Downloading:
This involves selecting .torrent files, downloading the contents from peers into local machine and running Data Integrity checks.  


## Set it up!

### For Uploading:

- python libtorrent used here.

[python-libtorrent requires python2 and has package manager support for only Debian.]
```
sudo apt install python-libtorrent
```
- To create the Message Digest of the contents, create a .torrent file of those contents and then start seeding them.
```
python2 Uploading/seed_final.py
```
( Specify the file/folder withing the Uploading directory as shown here & then let it seed indefinitely. A .torrent file will be created within the Uploading Directory)  
[Further work on posting to Google Drive] )

![](images/seeding.png)


### For Downloading:
- Install modules within requirements.txt
```
pip3 install -r requirements.txt 

```


Then run the BitTorrent Client GUI! (shown in image below).

```
python3 Downloading/bit-torrent/torrent_gui.py 
```
The process of running the GUI is shown here.
![](images/gui.png)

### Finally good to go!
Shown below is an image of the process of seeding contents, creating their .torrent file and adding this .torrent file into the BitTorrent GUI based client for downloading from peers.
![](images/download.png)



## Acknowledgments

* [Borzunov](https://github.com/borzunov/bit-torrent) - The Downloading portion of client! 

## Other


* [Torrents](https://eztv.io/) - Webpage to access larger, better seeded content.

