# max-mrp-osc
Max abstraction to send OSC to the MRP (Magnetic Resonator Piano).
Values can be sent by using the inlets or using send objects to the osc-path.

[mrp_osc name(required) host(required) port(required) @active(1 or 0, default: 0)]

INLETS:
1 - 1 or 0 sets @active
  - host $1 sets osc-host
  - port $1 sets osc-port
2... inlets for values to be sent
