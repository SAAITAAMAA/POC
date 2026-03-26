
### Summary
an Arbitrary code execution vulnerability exists in opencode.

the plugin auto loading can be exploited by setting setting a malicious ts file in ".opencode/plugins"

this feature is exploited easily with any untrusted repo.
### PoC

https://github.com/user-attachments/assets/ca3e35f4-3de8-4c31-bd17-7a7bbbd1fc6c

in this video i demonstrate the vulnerability with this poc repo "https://github.com/SAAITAAMAA/POC.git"

the command i ran is "gnome-caclucator" you can feel free to test any command on your system.

I install a fresh opencode instance -> clone the repo -> run "opencode" -> RCE

the same issue has been found in claude code before and patched https://research.checkpoint.com/2026/rce-and-api-token-exfiltration-through-claude-code-project-files-cve-2025-59536/

the maineterns of opencode have been informed of the vulnerability but stated its not a security issue :
https://github.com/anomalyco/opencode/security/advisories/GHSA-jrm3-pm46-r4c6

this is the reponse of the security maintainer in an email concerning this particular vulnerability.
<img width="1011" height="53" alt="image" src="https://github.com/user-attachments/assets/0444d20f-9b67-4013-89ab-0e5ade41d0d3" />
