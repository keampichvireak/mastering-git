## HEllo , GIT


-I'm adding this from 'feature-branch'


reg add "HKLM\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System\CredSSP\Parameters" /v AllowEncryptionOracle /t REG_DWORD /d 2 /f


# Trigger Machine Policy Retrieval
Invoke-WmiMethod -Namespace root\ccm -Class SMS_Client -Name TriggerSchedule -ArgumentList "{00000000-0000-0000-0000-000000000021}"

# Trigger Application Deployment Evaluation
Invoke-WmiMethod -Namespace root\ccm -Class SMS_Client -Name TriggerSchedule -ArgumentList "{00000000-0000-0000-0000-000000000121}"
