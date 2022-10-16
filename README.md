# Auto-File-Download-Using-JS

This script will help you to download your payload automatically into your targets system.

Steps - 

1 - Create Your Payload.

2 - Bring that payload into your Windows system.

3 - Open Powershell.

4 - Navigate to the directory where the paylaod is present.

5 - Commands to perform in Powershell - 
	
	1) (Get-Content C:\Windows\Desktop\Payload.exe)

	2) $base64string = [Convert]::ToBase64String([IO.File]::ReadAllBytes('C:\Windows\Desktop\Payload.exe'))

	3) $base64string | Out-File temporary.log

	4) code .\temporary.log

6 - Now copy the code into the index.html file.

7 - Now send index.html to your target and work done. Your payload will get downloaded automatically.

