#### Download a RPM package with all dependencies in CentOS
#### Please note that this plugin is applicable for "yum install/yum update" and not for "yum groupinstall". 
#### By default this plugin will download the latest available packages in the repository. You can however download a particular version by specifying the version.

yum install yum-plugin-downloadonly

yum install --downloadonly --downloaddir=<directory> <package-name> <package-name>

yum -y install /<directory>
