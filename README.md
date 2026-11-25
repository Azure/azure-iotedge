
```
        █████╗ ███████╗██╗   ██╗██████╗ ███████╗
       ██╔══██╗╚══███╔╝██║   ██║██╔══██╗██╔════╝
       ███████║  ███╔╝ ██║   ██║██████╔╝█████╗
       ██╔══██║ ███╔╝  ██║   ██║██╔══██╗██╔══╝
       ██║  ██║███████╗╚██████╔╝██║  ██║███████╗
       ╚═╝  ╚═╝╚══════╝ ╚═════╝ ╚═╝  ╚═╝╚══════╝
 ██╗         ████████╗    ███████╗██████╗  ██████╗ ███████╗
 ██║ ██████╗ ╚══██╔══╝    ██╔════╝██╔══██╗██╔════╝ ██╔════╝
 ██║██╔═══██║   ██║       █████╗  ██║  ██║██║  ███╗█████╗
 ██║██║   ██║   ██║       ██╔══╝  ██║  ██║██║   ██║██╔══╝
 ██║╚██████╔╝   ██║       ███████╗██████╔╝╚██████╔╝███████╗
 ╚═╝ ╚═════╝    ╚═╝       ╚══════╝╚═════╝  ╚═════╝ ╚══════╝
```

Welcome to the home of Azure IoT Edge, a product built from the open-source [IoT Edge project](https://github.com/azure/iotedge).

Azure IoT Edge moves cloud analytics and custom business logic to devices so that your organization can focus on business insights instead of data management. Enable your solution to truly scale by configuring your IoT software, deploying it to devices via standard containers, and monitoring it all from the cloud.

## Documentation
Documentation can be found at https://docs.microsoft.com/azure/iot-edge.

## LTS release cadence
Azure IoT Edge LTS releases follow the .NET LTS cadence. Each LTS release aligns its .NET components with a supported .NET LTS release and remains supported through the same end-of-support date. See the [Azure IoT Edge lifecycle](https://learn.microsoft.com/en-us/lifecycle/products/azure-iot-edge) and the [.NET support policy](https://dotnet.microsoft.com/en-us/platform/support/policy/dotnet-core) for details.

Current LTS support and release guidance:
* 1.5 LTS aligned with .NET 8 and reached end of support on Nov 10, 2026. (See the [.NET 8 support timeline](https://dotnet.microsoft.com/en-us/platform/support/policy/dotnet-core#dotnet-8).)
* 1.6 LTS aligns with .NET 10 LTS and is supported through Nov 14, 2028. (See the [.NET 10 support timeline](https://dotnet.microsoft.com/en-us/platform/support/policy/dotnet-core#dotnet-10).)
* We plan to release the next LTS approximately six months before the prior LTS reaches end of support to give customers time to upgrade.
* Customers still using 1.5 LTS should upgrade to 1.6 LTS.

## Release metadata maintenance

[product-versions.json](./product-versions.json) describes published product versions.
Its Docker image component `branch` fields determine which IoT Edge branch's
base image update pipeline checks those images.

* Keep 1.6 image components mapped to `release/1.6` in both the stable and LTS channels.
* 1.5 LTS is out of support and has been removed from the release metadata.
* When 1.7 is published, add its release metadata with image components mapped to `main`;
  do not change published 1.6 image versions merely because development moves to 1.7.
* API Proxy and Metrics Collector are independently versioned and remain mapped to `main`.

## Issues
Issues can be filed in the [issues section](https://github.com/azure/iotedge/issues) of the IoT Edge GitHub repo. Azure IoT Edge is built from the open-source IoT Edge project. Development and bug fixing happens in the repo of the open-source project.

## Feature requests
Feature requests can be filed on the [Azure IoT Edge User Voice page](https://feedback.azure.com/forums/907045-azure-iot-edge). 

## Data / Telemetry
IoT Edge sends basic metadata to Microsoft about the host device. This data may be used to improve Microsoft products and services. This data includes:

* CPU architecture
* Total memory
* Virtualized machine
* Kernel name
* Kernel release
* Kernel version
* OS name
* OS version
* OS variant
* OS build
* System Manufacturer
* System Product

To opt out, set the `DisableDeviceAnalyticsMetadata` [environment variable on EdgeAgent](https://github.com/Azure/iotedge/blob/main/doc/EnvironmentVariables.md).

To learn more about Microsoft policies, review the [privacy statement](https://go.microsoft.com/fwlink/?LinkId=521839&clcid=0x409).
