# Intune-Device-Management-Automation
Scripts and tools to automate device management tasks in Microsoft Intune. This can include enrolling devices, deploying applications, and configuring device compliance policies.


Project Outline:
•	README.MD: Detailed documentation on how to set up and use the automation scripts.
•	Scripts:
o	EnrollDevice.ps1: Script to enroll a device in Intune.
o	DeployApp.ps1: Script to deploy an application to devices.
o	ConfigureCompliance.ps1: Script to configure device compliance policies.




# Connect to MS Graph API
Connect-MSGraph

# Enroll a device in Intune
$device = New-IntuneManagedDeviceEnrollmentProfile -DisplayName "Corporate Device Enrollment" -Description "Profile for enrolling corporate devices" -Platform iOS -AuthenticationMode CompanyPortal

Write-Output "Device enrollment profile created: $($device.DisplayName)"
