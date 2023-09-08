# ICD Systems

[ICD Systems](https://www.icdsystems.com) is a [Crestron](https://www.crestron.com/) Service Provider (CSP), specalizing in enterprise scale and high-end residential development.

## ConnectCS

ConnectCS is a framework developed by ICD Systems to run control systems, and is compatible with Crestron 3-series and 4-series processors, as well as .NET Standard. ConnectCS supports different plugins loaded at runtime.

To actually use ConnectCS as a full program, you need a "Theme". Themes define the UI functionality of a system, and typically come bundled with the business logic to run rooms, etc.

A sample theme is provided, in the form of [ConnectPro](https://github.com/ICDSystems/ConnectPro). It includes a VTPro UI as well.

## XP3

[XP3](https://github.com/ICDSystems/XP3) is our implementation of "cross program crosspoints". The functionality closely resembles Crestron's traditional crosspoint symbols. It uses multicast for discovery between multiple programs, either on the same processor or different processors. It is useable in SimplWindows (with provided modules), or directly in S#Pro.

When written in C#, an XP3 equipment crosspoint can handle each connected control crosspoint independently, allowing multiple control devices to be connected at the same time but have different UIs. A popular use case for this is pagination, and allowing a panel to have an item "selected" independent of other panels.
