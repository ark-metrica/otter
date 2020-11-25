stage firmwares are based on 5772f24 

but with tweaks for reducing acceleration and deceleration
```
  tmc5130_writeInt(TMC5130, TMC5130_VSTART, 0);
  tmc5130_writeInt(TMC5130, TMC5130_A1, 1000);
  tmc5130_writeInt(TMC5130, TMC5130_V1, 50000);
  tmc5130_writeInt(TMC5130, TMC5130_AMAX, 1500);
  tmc5130_writeInt(TMC5130, TMC5130_VMAX, VMAX);
  tmc5130_writeInt(TMC5130, TMC5130_DMAX, 1500);
  tmc5130_writeInt(TMC5130, TMC5130_D1, 1000);
  tmc5130_writeInt(TMC5130, TMC5130_VSTOP, 10);
```

controller firmware is 19a521c
