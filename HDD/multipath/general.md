### Mount FC on node


#### show current PV
multipathd show paths format '%s %i %o %S' | awk -F'\\s+|:' 'NR>1 { print $1 " " $5 " " $7 }'| sort -u | sort -k1,1 -k2,2n


#### SSH GOTO node
mount | grep PodName

/dev/mapper/mpathh on /var/lib/kubelet/pods/dd5c8127-c98e-4344-95d3-62da593b3174/volumes/kubernetes.io~fc/grafana-pm 


#### create dir for mount
mkdir /mnt/SomeDirName


#### mount FC to local directory
mount /dev/mapper/mpathh /mnt/SomeDirName


# umount when finish work
sudo umount /mnt/SomeDirName
