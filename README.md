# Deeplink Reverse TCP

Things needed:
>* Microsoft word (preferably older versions)
>* Notepad/Notepad++
>* Kali VM
>* Windows reverse_tcp payload
>* Windows VM

## Payload Creation & C2 setup
1. Create a windows/meterpreter/reverse_tcp payload in kali linux
2. Start apache server
3. Push the payload.exe to var/www/html

## Modifying SettingContent-ms file in Windows
1. Open notepad/notepad++ and copy paste ILoveWindows.SettingContent-ms
2. Replace "http://192.168.225.129/pwn.exe" with your kali local ip and payload executable name
3. Save

## Inserting SettingContent-ms file in MSword
1. Open microsoft word and go to "Insert" -> "Object" -> "Create from file" -> Browse and select your SettingContent-ms file -> check both "Link to file" and "Display as icon" -> (Optional) change your icon and display name
