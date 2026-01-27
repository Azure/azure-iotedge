
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

Current LTS planning guidance:
* 1.5 LTS aligns with .NET 8 and is supported until .NET 8 reaches end of support on Nov 10, 2026. (See the [.NET 8 support timeline](https://dotnet.microsoft.com/en-us/platform/support/policy/dotnet-core#dotnet-8).)
* 1.6 LTS is planned to align with the supported .NET 10 LTS release and is expected to be supported for three years, through Nov 14, 2028. (See the [.NET 10 support timeline](https://dotnet.microsoft.com/en-us/platform/support/policy/dotnet-core#dotnet-10).)
* We plan to release the next LTS approximately six months before the prior LTS reaches end of support to give customers time to upgrade.
* Based on current plans, no major changes are expected between 1.5 LTS and 1.6 LTS, so upgrades should be straightforward.

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
