# uns-collector

## This is a repository that will install the uns-collector when used with ansible-pull

### Run the command ```sudo ansible-pull -U https://github.com/unsinc/uns-collector.git``` to have the following done on the system:

1.  This will install the following packages onto an Ubuntu/Debian System
  - auditd
  - htop
  - nano
  - psmisc
  - net-tools

1.  This will expand the ubuntu-lv to the full size allocated
1.  Several Cron Jobs are added to keep the sensor current
	-  Collector Configuration: @ Every Hour at 10 after the hour every day

1.  The system looks to keep itself up-to-date with security updates
	-  **This system will reboot itself if required by the updates @ 08:00 UTC**