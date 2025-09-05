# Refresh all policies
Invoke-WmiMethod -Namespace root\ccm -Class SMS_Client -Name ResetPolicy 1
# Trigger policy evaluation
Invoke-WmiMethod -Namespace root\ccm -Class SMS_Client -Name TriggerSchedule -ArgumentList "{00000000-0000-0000-0000-000000000021}"
Remove-Item "C:\Windows\ccmcache" -Recurse -Force
rmdir C:\Windows\ccmcache /s /q
rmdir C:\Windows\ccmcache /s /q
https://chatgpt.com/s/t_68ba6f532b44819193ca4f2a64bf439f
