<img src="Design/wilderness-labs-banner.jpg"  alt="Meadow.ProjectLab, C#, iot" style="margin-bottom:10px" />

Welcome to the Wilderness Labs GitHub home! Here you will find our device platform code. It is nearly completely open and we're working on cleaning up and opening the remaining bits.

## Contents
* [Meadow Software Stack](#meadow-software-stack)
* [Managed Meadow.IoT Platform Stack](#managed-meadowiot-platform-stack)
* [Repo Status](#repo-status)
    * [Meadow.Core Repos](#meadowcore-repos)
    * [Meadow.Foundation Repos](#meadowfoundation-repos)
    * [Tooling](#tooling)
    * [IoT Accelerator Repos](#iot-accelerator-repos)
    * [Project Samples](#project-samples)
* [Support](#support)

## Meadow Software Stack

The following diagram illustrates the layers of the device platform:

![Illustration fo the Wilderness Labs IoT Platform stack including Meadow.Foundation (with an associated sensor code sample), Meadow.Core (with a sample hardware API), and the OS services layer including things like sleep APIs, health-monitoring, etc.](./Design/Platform_Stack.png)

For a more complete understanding of the platform, please check out our [developer documentation](http://developer.wildernesslabs.co/).

## Managed Meadow.IoT Platform Stack

The managed portion of the Meadow.IoT stack includes the following layers:
* **Meadow.Core** - Contains the hardware APIs and userland services that run on Meadow.OS and other .NET capable operating systems and expose the underlying hardware and platform services.
* **Meadow.Foundation** - Peripheral drivers and libraries that run on Meadow.Core and provides plug-and-play APIs for sensors, motors, displays, etc., as well as high level libraries for working with hardware devices. For a full list of supported peripherals and included libraries refer to [this page](https://developer.wildernesslabs.co/Meadow/Meadow.Foundation/Peripherals/). 

## Repo Status

### Meadow.Core Repos

| Repo | Nuget | `Main` Branch | `Develop` Branch |
|-------------------|--|--|--| 
| [![Meadow.Units](https://badgen.net/badge/Repository/Meadow.Units/blue?icon=github)](https://github.com/WildernessLabs/Meadow.Units)             | [![NuGet Badge](https://buildstats.info/nuget/Meadow.Units)](https://www.nuget.org/packages/Meadow.Units)         | [![Main Branch](https://github.com/WildernessLabs/Meadow.Units/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Units/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Meadow.Logging/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Logging/actions/workflows/develop-ci.yml) |
| [![Meadow.Logging](https://badgen.net/badge/Repository/Meadow.Logging/blue?icon=github)](https://github.com/WildernessLabs/Meadow.Logging)       | [![NuGet Badge](https://buildstats.info/nuget/Meadow.Logging)](https://www.nuget.org/packages/Meadow.Logging)     | [![Main Branch](https://github.com/WildernessLabs/Meadow.Logging/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Logging/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Meadow.Units/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Units/actions/workflows/develop-ci.yml) |
| [![Meadow.Contracts](https://badgen.net/badge/Repository/Meadow.Contracts/blue?icon=github)](https://github.com/WildernessLabs/Meadow.Contracts) | [![NuGet Badge](https://buildstats.info/nuget/Meadow.Contracts)](https://www.nuget.org/packages/Meadow.Contracts) | [![Main Branch](https://github.com/WildernessLabs/Meadow.Contracts/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Contracts/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Meadow.Contracts/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Contracts/actions/workflows/ci-develop-push.yml) |
| [![Meadow.Core](https://badgen.net/badge/Repository/Meadow.Core/blue?icon=github)](https://github.com/WildernessLabs/Meadow.Core)                | [![NuGet Badge](https://buildstats.info/nuget/Meadow)](https://www.nuget.org/packages/Meadow)                     | [![Main Branch](https://github.com/WildernessLabs/Meadow.Core/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Core/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Meadow.Core/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Core/actions/workflows/develop-ci.yml) |
| [![Meadow.Modbus](https://badgen.net/badge/Repository/Meadow.Modbus/blue?icon=github)](https://github.com/WildernessLabs/Meadow.Modbus)          | [![NuGet Badge](https://buildstats.info/nuget/Meadow.Modbus)](https://www.nuget.org/packages/Meadow.ModBus)       | [![Main Branch](https://github.com/WildernessLabs/Meadow.Modbus/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Modbus/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Meadow.Modbus/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Modbus/actions/workflows/develop-ci.yml) |
| [![MQTTnet](https://badgen.net/badge/Repository/MQTTnet/blue?icon=github)](https://github.com/WildernessLabs/MQTTnet)                            | [![NuGet Badge](https://buildstats.info/nuget/Meadow.MQTT)](https://www.nuget.org/packages/Meadow.MQTT)           |  |  |

### Meadow.Foundation Repos

| Repo | `Main` Branch | `Develop` Branch |
|-------------------|--|--| 
| [![Meadow.Foundation](https://badgen.net/badge/Repository/Meadow.Foundation/blue?icon=github)](https://github.com/WildernessLabs/Meadow.Foundation) | [![Main Branch](https://github.com/WildernessLabs/Meadow.Foundation/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Foundation/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Meadow.Foundation/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Foundation/actions/workflows/develop-ci.yml) |
| [![Meadow.Foundation.MBus](https://badgen.net/badge/Repository/Meadow.Foundation.MBus/blue?icon=github)](https://github.com/WildernessLabs/Meadow.Foundation.MBus) | [![Main Branch](https://github.com/WildernessLabs/Meadow.Foundation.MBus/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Foundation.MBus/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Meadow.Foundation.MBus/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Foundation.MBus/actions/workflows/develop-ci.yml) |
| [![Meadow.Foundation.Grove](https://badgen.net/badge/Repository/Meadow.Foundation.Grove/blue?icon=github)](https://github.com/WildernessLabs/Meadow.Foundation.Grove) | [![Main Branch](https://github.com/WildernessLabs/Meadow.Foundation.Grove/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Foundation.Grove/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Meadow.Foundation.Grove/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Foundation.Grove/actions/workflows/develop-ci.yml) |
| [![Meadow.Foundation.mikroBUS](https://badgen.net/badge/Repository/Meadow.Foundation.mikroBUS/blue?icon=github)](https://github.com/WildernessLabs/Meadow.Foundation.mikroBUS) | [![Main Branch](https://github.com/WildernessLabs/Meadow.Foundation.mikroBUS/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Foundation.mikroBUS/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Meadow.Foundation.mikroBUS/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Foundation.mikroBUS/actions/workflows/develop-ci.yml) |
| [![Meadow.Foundation.FeatherWings](https://badgen.net/badge/Repository/Meadow.Foundation.FeatherWings/blue?icon=github)](https://github.com/WildernessLabs/Meadow.Foundation.FeatherWings) | [![Main Branch](https://github.com/WildernessLabs/Meadow.Foundation.FeatherWings/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Foundation.FeatherWings/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Meadow.Foundation.FeatherWings/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Foundation.FeatherWings/actions/workflows/develop-ci.yml) |
| [![Meadow.Foundation.CompositeDevices](https://badgen.net/badge/Repository/Meadow.Foundation.CompositeDevices/blue?icon=github)](https://github.com/WildernessLabs/Meadow.Foundation.CompositeDevices) | [![Main Branch](https://github.com/WildernessLabs/Meadow.Foundation.CompositeDevices/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Foundation.CompositeDevices/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Meadow.Foundation.CompositeDevices/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Foundation.CompositeDevices/actions/workflows/develop-ci.yml) |
| [![Meadow.Foundation.Web.Maple](https://badgen.net/badge/Repository/Meadow.Foundation.Web.Maple/blue?icon=github)](https://github.com/WildernessLabs/Maple) | [![Main Branch](https://github.com/WildernessLabs/Maple/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Maple/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Maple/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Maple/actions/workflows/develop-ci.yml) |

### Tooling

The tooling stack includes both the CLI source as well as the IDE extensions.

| Repo |
|------------|
| [![Meadow.CLI](https://badgen.net/badge/Repository/Meadow.CLI/blue?icon=github)](https://github.com/WildernessLabs/Meadow.CLI) |
| [![VS_Win_Meadow_Extension ](https://badgen.net/badge/Repository/VS_Win_Meadow_Extension/blue?icon=github)](https://github.com/WildernessLabs/VS_Win_Meadow_Extension) |
| [![VS_Mac_Meadow_Extension ](https://badgen.net/badge/Repository/VS_Mac_Meadow_Extension/blue?icon=github)](https://github.com/WildernessLabs/VS_Mac_Meadow_Extension) |
| [![VSCode_Meadow_Extension ](https://badgen.net/badge/Repository/VSCode_Meadow_Extension/blue?icon=github)](https://github.com/WildernessLabs/VSCode_Meadow_Extension) |


### IoT Accelerator Repos

All of the IoT accelerator designs can be found below:

| Repo | Nuget | `Main` Branch | `Develop` Branch |
|-------------------------|--|--|--| 
| [![Meadow.Clima](https://badgen.net/badge/Repository/Clima/blue?icon=github)](https://github.com/WildernessLabs/Clima) | [![NuGet Badge](https://buildstats.info/nuget/Meadow.Clima)](https://www.nuget.org/packages/Meadow.Clima) | [![Main Branch](https://github.com/WildernessLabs/Clima/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Clima/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Clima/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Clima/actions/workflows/develop-ci.yml) |
| [![Meadow.Juego](https://badgen.net/badge/Repository/Juego/blue?icon=github)](https://github.com/WildernessLabs/Juego) | [![NuGet Badge](https://buildstats.info/nuget/Meadow.Juego)](https://www.nuget.org/packages/Meadow.Juego) | [![Main Branch](https://github.com/WildernessLabs/Juego/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Juego/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Juego/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Juego/actions/workflows/develop-ci.yml) |
| [![Meadow.ProjectLab](https://badgen.net/badge/Repository/Meadow.ProjectLab/blue?icon=github)](https://github.com/WildernessLabs/Meadow.ProjectLab) | [![NuGet Badge](https://buildstats.info/nuget/Meadow.ProjectLab)](https://www.nuget.org/packages/Meadow.ProjectLab) | [![Main Branch](https://github.com/WildernessLabs/Meadow.ProjectLab/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.ProjectLab/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Meadow.ProjectLab/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.ProjectLab/actions/workflows/develop-ci.yml) |
| [![Meadow.GNSS_Sensor_Tracker](https://badgen.net/badge/Repository/GNSS_Sensor_Tracker/blue?icon=github)](https://github.com/WildernessLabs/GNSS_Sensor_Tracker) | [![NuGet Badge](https://buildstats.info/nuget/Meadow.GnssTracker)](https://www.nuget.org/packages/Meadow.GnssTracker) | [![Main Branch](https://github.com/WildernessLabs/GNSS_Sensor_Tracker/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/GNSS_Sensor_Tracker/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/GNSS_Sensor_Tracker/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/GNSS_Sensor_Tracker/actions/workflows/develop-ci.yml) |

### Project Samples

| Repo | `Main` Branch | `Develop` Branch |
|-----------------|--|--|
| [![Juego.Samples](https://badgen.net/badge/Repository/Juego.Samples/blue?icon=github)](https://github.com/WildernessLabs/Juego.Samples) | [![Main Branch](https://github.com/WildernessLabs/Juego.Samples/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Juego.Samples/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Juego.Samples/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Juego.Samples/actions/workflows/develop-ci.yml) |
| [![Meadow.Core.Samples](https://badgen.net/badge/Repository/Meadow.Core.Samples/blue?icon=github)](https://github.com/WildernessLabs/Meadow.Core.Samples) | [![Main Branch](https://github.com/WildernessLabs/Meadow.Core.Samples/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Core.Samples/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Meadow.Core.Samples/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Core.Samples/actions/workflows/develop-ci.yml) |
| [![Meadow.Cloud.Samples](https://badgen.net/badge/Repository/Meadow.Cloud.Samples/blue?icon=github)](https://github.com/WildernessLabs/Meadow.Cloud.Samples) | [![Main Branch](https://github.com/WildernessLabs/Meadow.Cloud.Samples/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Cloud.Samples/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Meadow.Cloud.Samples/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Cloud.Samples/actions/workflows/develop-ci.yml) |
| [![Meadow.Project.Samples](https://badgen.net/badge/Repository/Meadow.Project.Samples/blue?icon=github)](https://github.com/WildernessLabs/Meadow.Project.Samples) | [![Main Branch](https://github.com/WildernessLabs/Meadow.Project.Samples/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Project.Samples/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Meadow.Project.Samples/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Project.Samples/actions/workflows/develop-ci.yml) |
| [![Meadow.Desktop.Samples](https://badgen.net/badge/Repository/Meadow.Desktop.Samples/blue?icon=github)](https://github.com/WildernessLabs/Meadow.Desktop.Samples) | [![Main Branch](https://github.com/WildernessLabs/Meadow.Desktop.Samples/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Desktop.Samples/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Meadow.Desktop.Samples/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.Desktop.Samples/actions/workflows/develop-ci.yml) |
| [![Meadow.ProjectLab.Samples](https://badgen.net/badge/Repository/Meadow.ProjectLab.Samples/blue?icon=github)](https://github.com/WildernessLabs/Meadow.ProjectLab.Samples) | [![Main Branch](https://github.com/WildernessLabs/Meadow.ProjectLab.Samples/actions/workflows/main-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.ProjectLab.Samples/actions/workflows/main-ci.yml) | [![Develop Branch](https://github.com/WildernessLabs/Meadow.ProjectLab.Samples/actions/workflows/develop-ci.yml/badge.svg)](https://github.com/WildernessLabs/Meadow.ProjectLab.Samples/actions/workflows/develop-ci.yml) |

## Support

Found any bugs or issues in one of our repos? 
* File an [issue](https://github.com/WildernessLabs/Meadow.Desktop.Samples/issues) with a repro case to investigate, and/or
* Join our [public Slack](http://slackinvite.wildernesslabs.co/), where we have an awesome community helping, sharing and building amazing things using Meadow.