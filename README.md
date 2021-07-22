# CVE-2021-36934
CVE-2021-36934 PowerShell Fix

This powershell script fixes CVE-2021-36934, based on the original script of Joran Slingerland (https://github.com/JoranSlingerland)
https://github.com/JoranSlingerland/CVE-2021-36934/blob/main/CVE-2021-36934.ps1

The Powershell script will do following:

- Produce a LOG under $env:windir\Logs\ with the name of CVE-2021-36934_$date.$time.log
- Check if the vulnerability is present
- Check if ShadowCopies are present, and if present delete them
- Fix the ACL on the $env:windir\system32\config\ folder
- Recreate Shadowcopies (if they where present)

Also a Baseline for MECM is present
