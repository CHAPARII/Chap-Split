# Split Mechanical Keyboard

The keyboard uses a split layout with around 76 keys, The design is meant to be customizable and DIY-friendly. It uses Kailh hot-swap sockets, which means switches can be replaced anytime without needing to desolder them. This makes it easy to experiment with different switches later. For the controller, I used the nRF52840 development board, which works well with ZMK firmware. ZMK alows the keyboard to support Bluetooth, so it can be used wirelessly. It also support customizable keymaps, layers, and other advanced keyboard features. 

Designing the PCB took a lot more time than I expected. there were many small issues during routing and schematic checks. I spent quite a lot of time fixing different problems and improving the layout. After several iterations and debugging, the **PCB now finally passes both DRC (Design Rule Check) and ERC (Electrical Rule Check) with 0 errors**. Fixing all those issues took a lot of effort, but it was really satisfying to finally see everything clean in KiCad. The keyboard uses 76 mechanical switches, and each switch has a 1N4148 diode for the key matrix. Stabilizers are used for larger keys, and the switches are mounted using Kailh hot-swap sockets. Keycaps and switchs can be changed depending on personal preference.

One goal of this project was also to keep the build relatively affordable. Based on the current Bill of Materials, the estimated total cost is around ₹11,174 (~$121.54 USD) including PCB manufacturing and other components. I tried my best to keep it in budget, I tried to get maximum thing from one place (amazon) in budget to make things simple and save in shipping charges. Also I'll buy the PCBs locally and it would cost me around $20.

Overall, this project was mainly built for learning, experimenting, and having fun with hardware design. It was a really good experience going through the full PCB design process and understanding how keyboards work internally. If someone finds this project interesting or wants to build their own version of it, that would be really awesome.

## 📦 Bill of Materials (BOM) – Split Keyboard

| # | Component | Quantity | Unit Price | Total | Link |
|---|-----------|---------|-----------|------|------|
| 1 | Kailh Hot-Swap Sockets | 1 pack (~100 pcs) | ₹2124 | ₹2124 | https://www.amazon.in/gp/product/B0GHR248QJ |
| 2 | Mechanical Switches | 76 (1 pack) | ₹1965 | ₹1965 | https://www.amazon.in/gp/product/B0F53HLG5M |
| 3 | Stabilizers | 2 sets | ₹876 | ₹1752 | https://www.amazon.in/gp/product/B0FRN1CF4Q |
| 4 | Keycaps | 2 sets | ₹852 | ₹1704 | https://www.amazon.in/gp/product/B0F3883M9C |
| 5 | 1N4148 Diodes | 1 pack (~100 pcs) | ₹285 | ₹285 | https://www.amazon.in/gp/product/B0FJLP12GX |
| 6 | nRF52840 Microcontroller | 2 | ₹758 | ₹1516 | https://robu.in/product/promicro-nrf52840-development-board/ |
| 7 | PCB (Will buy it locally) | 1 order (2PCB) | $20 | ≈ ₹1838 | — |

---
### 💰 Total Estimated Cost

| Item | Cost |
|-----|------|
| Components Total | ₹9,336 |
| PCB | ≈ ₹1,838 |
| **Total Build Cost** | **≈ ₹11,174** (**$121.54 USD**) |