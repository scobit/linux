### VM logs spam 

/var/log/messages
var/log/syslog

multipathd[651]: sda: add missing path
multipathd[651]: sda: failed to get udev uid: Invalid argument
multipathd[651]: sda: failed to get sysfs uid: Invalid argument
multipathd[651]: sda: failed to get sgio uid: No such file or directory
multipathd[651]: sda: add missing path
multipathd[651]: sda: failed to get udev uid: Invalid argument
multipathd[651]: sda: failed to get sysfs uid: Invalid argument
multipathd[651]: sda: failed to get sgio uid: No such file or directory

### Fix

#### Edit configuration (add blacklist)
vim /etc/multipath.conf

defaults {
    user_friendly_names yes
}

blacklist {
    device {
        vendor "VMware"
        product "Virtual disk"
    }
}

#### Restart the multipath-tools service
systemctl restart multipath-tools
/etc/init.d/multipath-tools restart
