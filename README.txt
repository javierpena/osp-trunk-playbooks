* We start with a RHEL 7 VM, with the following repos enabled:

sudo subscription-manager repos --enable rhel-7-server-rpms 
sudo subscription-manager repos --enable rhel-7-server-rh-common-rpms 
sudo subscription-manager repos --enable rhel-7-server-optional-rpms 
sudo subscription-manager repos --enable rhel-7-server-extras-rpms
sudo subscription-manager repos --enable rhel-7-server-openstack-12-rpms    # required for puppet 4.x RPMs

* And EPEL, because we will need it for Mock (?!):

sudo yum install https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm


