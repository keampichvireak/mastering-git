# Refresh all policies
Invoke-WmiMethod -Namespace root\ccm -Class SMS_Client -Name ResetPolicy 1
# Trigger policy evaluation
Invoke-WmiMethod -Namespace root\ccm -Class SMS_Client -Name TriggerSchedule -ArgumentList "{00000000-0000-0000-0000-000000000021}"
