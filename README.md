# Install_RSAT_for_v1809+
Automated install for RSAT (Remote Server Administration Tools) in Windows 10 1809 and newer.


RSAT (Remote Server Administration Tools) in Windows 10 v1809 and v1903 are no longer a downloadable add-on to Windows. Instead its included as a set of  "Features on Demand" directly in Windows.

The script will only run on Windows 10 v1809 or v1903.

The script requires administrative rights as well as access to the Internet (RSAT is installed through Microsoft Update).

The script is built around Get-WindowsCapability, Add-WindowsCapability and Remove-WindowsCapability.

The script comes with 4 options:

.\Install-RSATv1809v1903.ps1 -All (-All is installing ALL the features within the RSAT bundle)
.\Install-RSATv1809v1903.ps1 -Basic (-Basic is only installing AD DS, DHCP, DNS, Group Policy Management and Server Manager)
.\Install-RSATv1809v1903.ps1 -ServerManager (-ServerManager is only installing the Server Manager)
.\Install-RSATv1809v1903.ps1 -Uninstall (-Uninstall removes all RSAT features again)
