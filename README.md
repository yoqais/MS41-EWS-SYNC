# MS41-EWS-SYNC
This guide will show you how to properly sync your E36's EWS to your ECU - avoiding EWS Deletes or messy wiring

---

## 🧰 Prerequisite
- ⚡ INPA 5.0.6

---
⚡OBD2 port & x20 Diag Connector (Female):
-Connect Pin 14 to Pin 18 to put the ECU in Write mode
-Connect Pin 2 to Pin 17 to bridge the OBD2 port in the car to the ECU which enables flashing via obd2 port inside the car
---
---
2. Open INPA:
Navigate to:
```bash
Older/Special Models ->E36->Engine->MS41.1/2
```
---
Click F3 and go to Coding section.
**take note of your ISN for EWS. should look like "c26" for example. it is case sensitive.
![INPA SCREENSHOT](https://github.com/yoqais/MS41-EWS-SYNC/blob/main/INPA_ENGINE_CODING.jpg?raw=true)

Navigate to:
```bash
Older/Special Models ->E36>Body->ELectronic vehicle immobilization EWS
```
1. Press f6 to open the CODING screen
2. Press f1 to open the ACTIVATE screen. You'll see a number highlighted. It will be in the format of 0x26c.
3. Erase it.
4. Type in your ISN using that format. If it's c26 type 0x26c or just type c26 without the 0x. Both have successfully worked. Press ENTER
5. Close INPA and turn your ignition off for 30 seconds. Restart your car and EWS should be aligned!
---
