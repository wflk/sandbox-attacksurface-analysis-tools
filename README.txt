sandbox-attacksurface-analysis-tools

(c) Google Inc. 2015
Developed by James Forshaw

This is a small suite of tools to test various properties of sandboxes on Windows. Many of the checking
tools take a -p flag which is used to specify the PID of a sandboxed process. The tool will impersonate
the token of that process and determine what access is allowed from that location. Also it's recommended
to run these tools as an administrator or local system to ensure the system can be appropriately enumerated.

CheckDeviceAccess : Check access to device objects
CheckExeManifest: Check for specific executable manifest flags
CheckFileAccess: Check access to files
CheckObjectManagerAccess: Check access to object manager objects
CheckProcessAccess: Check access to processes
CheckResistryAccess: Check access to registry
CheckNetworkAccess: Check access to network stack
DumpTypeInfo: Dump simple kernel object type information
DumpProcessMitigations: Dump basic process mitigation details on Windows8+
NewProcessFromToken: Create a new process based on existing token
ObjectList: Dump object manager namespace information
TokenView: View and manipulate various process token values

The tools can be built with Visual Studio 2013