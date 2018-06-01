##On Ubuntu
`sudo nano /etc/exports`

Insert:

`/home/martin    192.168.1.0/24(rw,all_squash,no_root_squash,insecure,anonuid=1000,anongid=1000,no_subtree_check)`

Run

`sudo exportfs -vra`

## On OSX

https://coderwall.com/p/fuoa-g/automounting-nfs-share-in-os-x-into-volumes

