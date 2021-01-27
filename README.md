# material-inventory-api-server-daemon

How to install

Rename the path to the golang build server file location
SCRIPT=<PATH>

Rename PID and LOG name 
PIDFILE=/var/run/<NAME>.pid
LOGFILE=/var/log/<NAME>.log

Rename the service name

Copy to /etc/init.d:

cp "misapidaemon.sh" "/etc/init.d/misapidaemon"
chmod +x /etc/init.d/misapidaemon

Start and test your service and install the service to be run at boot-time:
service coolserver start
service coolserver stop
update-rc.d coolserver defaults
