# mrp.osc

Max abstraction to send OSC to the MRP (Magnetic Resonator Piano).
Values can be sent by sending a OSC message into the inlet.
The mrp.osc object validates the OSC path, but NOT the message arguments. The helpfile contains a list of all viable paths and the arguments expected by the mrp.
The mrp.osc object does monitor or limit the speed at which OSC messages are sent.

Open the help-patcher for more information.

## Installation
Download or clone this repo into "/Path-to-Max-Folder/Max 8/Packages/mrp.osc".

Example (Mac OS):
```
cd ~/Documents/Max\ 8/Packages
git clone https://github.com/michaelmariaott/mrp.osc.git
```

## Reference

```
[mrp_osc host (opt) port (opt) @active (1 or 0, default: 0)]
```

INLET:
```
1: - 0 or int sets @active
   - "host $1" sets osc-host
   - "port $1" sets osc-port
   - anything: sent as OSC Message to the MRP. Format: "/path values"
```

OUTLET:
```
1: status messages
```
