# Cap Touch Picture Frame (CapFrame32)
An ESP32 Powered Capacitive touch panel for ESPHome and Home Assistant

The Problem: I want to be able to control home assiatnt from many rooms in the house. Placing tablets in each room is too expensive their cords hanging are unsightly and outlets are not always convieniently placed. The solution also has to match the decore of each room and blend into the space.

The Soltuion: CapFrame32 provides a battery powered solution that can match the decore of any room. The ESP32 is in deep sleep and wakes up with a users touch to one of the capacitive areas. Based on which  The unit can be flashed from ESPHome, Tasmota, or white your own software. The esp32 can be updated over the air once soldered to the board.

-   🔋   Battery Powered (1-18650)
-  🏪 Uses standard 4"x6" picture frames
-  3️⃣ components to solder
-  3️⃣ objects to 3D print. No support and about 1 hour of print time.

   CapFrame32 can be mounted on small picture nails or adhesive hangers. It's very light.
   
<img src="https://i.imgur.com/jh7MDC7.jpg" alt="CapFrame32" width="400"/>
<img src="https://imgur.com/JvT1Y4J.jpg" alt="CapFrame32" width="400"/>
<img src="https://imgur.com/y9FOEVh.jpg" alt="ESP32-Wroom-32D Programmer" width="400"/>
<img src="https://imgur.com/qYsWsX9.jpg" alt="Front of Board" width="400"/>
<img src="https://imgur.com/SVfPY0e.jpg" alt="Back of Board" width="400"/>
   
Shopping List:
 - 1 - 4x6 picture frame - Walmart has them for $2.50
 - 1 - 18650 battery [18650BatteryStore](https://www.18650batterystore.com/collections/18650-batteries)
 - 1 - ESP32-Wroom-32D - [Amazon non-affiliant link](https://www.amazon.com/gp/product/B085BNHPW5/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1)
 - 2 - 18650 battery holders. [digikey](https://www.digikey.com/en/products/detail/keystone-electronics/254/9646025) - You need 2 per board

Instructions
 - Order the circuit boards from a pcb manufacturer (JLCPCB, PCBWay, etc...) I order them in white so the board doesn't show through
 - [Download](https://github.com/Therefore/Cap-Touch-Picture-Frame/blob/main/Wall%20Offset%20Mounts.stl) and print the 3D parts
 - [Download](https://github.com/Therefore/Cap-Touch-Picture-Frame/blob/main/CapFrame32%20-%20Paper%20Template.pptx), customize, and print the paper template
 - Use ESPHome (or Tasmota or your own) to flash the ESP32 Chip. I use one of [these](https://i.imgur.com/y9FOEVh.jpg).
 - Solder the ESP32 chip and battery holder to the board
 - Place the components in a 4" x 6" picture frame that matches your decor
 - Power it up by putting in the battery!

Next Versions:
 - Choice power by 18650 or MicroUSB
 - Optional JST-2 connector for prismatic cells would give slimmer profile
 - voltage divider to ADC-0 would give an additional sensor about battery life.

Troubleshooting
 Chip doesn't boot up?
 - Ensure you're soldering the GND, VIN, and EN pins on the ESP32.
