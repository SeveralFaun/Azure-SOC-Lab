# Azure-SOC-Lab

SOC Environment built in Microsoft Azure

## Architecture

Isolated Resource Group, containing a single Vnet. A Windows 10 VM is hosted in the Vnet, with the NSG tuned to allow traffic from any port. A LAW uses the VM as a log source, and Sentinel and Defender are used to query logs for malicious traffic, create alert rules, and create workbooks and watchlists.
