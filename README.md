# Apollo mmWave CO2 Multisensor (MSR-2) ld2410

<img width="1083" alt="image" src="https://github.com/ApolloAutomation/MSR-2/assets/24777085/63cdafa0-2572-44a0-b7fa-dabc629c93ef">



This sensor offers a wide range of functionality for Home Assistant in a very tiny package.

YAML Files:
- MSR-2.yaml: This file is a minimal config. It doesn't have the bluetooth or OTA components. Use this if you are looking to add BLE proxy or BLE tracking.
- MSR-2_BLE.yaml: This file contains BLE proxy code. We use it as an automated test during our build process. But can be an example for adding BLE proxy to your device.
- MSR-2_Factory.yaml: This is the firmware flashed by us on new devices. It contains the components for ESP improve, allowing easy adoption in Home Assistant. When you load the device in ESPHome addon, it will grab the firmware from MSR-2.yaml which no longer has the improve.

Links: \
Discord (Support/feedback/discussion/future products): [https://discord.gg/8PpS4yUaUh](https://discord.gg/mMNgQPyF94) \
Shop: [https://apolloautomation.com](https://apolloautomation.com/products/msr-2) \
Wiki: https://wiki.apolloautomation.com \
3D Files: [https://www.printables.com/model/932026-apollo-automation-msr-2-mmwave-co2-multisensor-for](https://www.printables.com/model/932026-apollo-automation-msr-2-mmwave-co2-multisensor-for)
