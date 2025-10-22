# MS41-EWS-SYNC
This guide will show you how to properly sync your E36's EWS to your ECU - avoiding EWS Deletes or messy wiring

---

## 🧰 Prerequisite
- ⚡ INPA 5.0.6
---
1. Open INPA:
Navigate to:
```bash
Older/Special Models ->E36>Engine->MS41.1/2
```
---
Click F3 and go to Coding section.
**take note of your ISN for EWS. should look like "a42" it is case sensitive.
![alt text](https://github.com/yoqais/MS41-EWS-SYNC/blob/main/INPA_ENGINE_CODING.jpg?raw=true)

Navigate to:
```bash
Older/Special Models ->E36>Body->ELectronic vehicle immobilization EWS
```
1. Press f6 to open the CODING screen
2. Press f1 to open the ACTIVATE screen. You'll see a number highlighted. It will be in the format of 0x42a.
3. Erase it.
4. Type in your ISN using that format. If it's a42 type 0x42a or just type a42 without the 0x. Both have successfully worked. Press ENTER
5. Close INPA and turn your ignition off for 30 seconds. Restart your car and EWS should be aligned!
---
