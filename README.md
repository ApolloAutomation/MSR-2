# Apollo mmWave CO2 Multisensor (MSR-2) ld2410

<img width="1083" alt="image" src="https://github.com/ApolloAutomation/MSR-2/assets/24777085/63cdafa0-2572-44a0-b7fa-dabc629c93ef">



This sensor offers a wide range of functionality for Home Assistant in a very tiny package.

YAML Files:
- MSR-2.yaml: This file is a minimal config. It doesn't have the bluetooth or OTA components. Use this if you are looking to add BLE proxy or BLE tracking.
- MSR-2_BLE.yaml: This file contains BLE proxy code. We use it as an automated test during our build process. But can be an example for adding BLE proxy to your device.
- MSR-2_Factory.yaml: This is the firmware flashed by us on new devices. It contains the components for ESP improve, allowing easy adoption in Home Assistant. When you load the device in ESPHome addon, it will grab the firmware from MSR-2.yaml which no longer has the improve.

Light sensor:
Newer MSR-2 boards use an LTR-303ALS ambient light sensor in place of the discontinued LTR-390UV. The same firmware runs on both. At boot it detects which sensor is fitted and shows only that sensor's entities:
- LTR-390UV boards: **LTR390 Light** and **LTR390 UV Index**, unchanged from earlier firmware.
- LTR-303ALS boards: **LTR303 Light**. The LTR-303ALS has no UV sensor, so these boards have no UV Index entity.
- If neither sensor answers at boot, the firmware hides nothing. All light sensor entities stay visible and read Unknown. This usually means a hardware fault.

The **Light Sensor Model** diagnostic entity shows which sensor your board has (`LTR-390UV` or `LTR-303ALS`), or `Not detected` if neither answered. When a sensor is detected, the device logs show an error for the model your board doesn't have, ending in "marked FAILED: not fitted (expected)". On LTR-390UV boards a "Communication failed" line for the LTR-303 driver comes just before it. Both are normal.

Links: \
Discord (Support/feedback/discussion/future products): [https://dsc.gg/ApolloAutomation] \
Shop: [https://apolloautomation.com](https://apolloautomation.com/products/msr-2) \
Wiki: https://wiki.apolloautomation.com \
3D Files: [https://www.printables.com/model/932026-apollo-automation-msr-2-mmwave-co2-multisensor-for](https://www.printables.com/model/932026-apollo-automation-msr-2-mmwave-co2-multisensor-for)
