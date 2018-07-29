# securitynews

WINDOWS DEFENDER RESEARCH announced the latest multi-tire attack on the supply chain.

Attackers compromised the shared infrastructure in the area between the vendor of a PDF editor application and one among its software program vendor partners, making the app’s legitimate installer the unsuspecting carrier of a malicious payload.


Windows Defender ATP was detecting and blockading a coin mining manner masquerading as pagefile.sys, which became being launched by way of a provider named xbox-service.exe. windows Defender ATP’s alert timeline showed that Xbox-service.exe turned into mounted via an installer bundle that became robotically downloaded from a suspicious remote server.
Software vendors and developers need to ensure they produce secure as well as useful software and services. To do that, we recommend:

Maintain a highly secure build and update infrastructure.
Immediately apply security patches for OS and software.
Implement mandatory integrity controls to ensure only trusted tools run.
Require multi-factor authentication for admins.
Build secure software updates as part of the software development lifecycle.
Require SSL for update channels and implement certificate pinning.
Sign everything, including configuration files, scripts, XML files, and packages.
Check for digital signatures, and don’t let the software updater accept generic input and commands.
Develop an incident response process for supply chain attacks.
Disclose supply chain incidents and notify customers with accurate and timely information.
https://cloudblogs.microsoft.com/microsoftsecure/2018/07/26/attack-inception-compromised-supply-chain-within-a-supply-chain-poses-new-risks/ 

Indicators of compromise (IOCs)

Malicious MSI font packages:

– a69a40e9f57f029c056d817fe5ce2b3a1099235ecbb0bcc33207c9cff5e8ffd0
– ace295558f5b7f48f40e3f21a97186eb6bea39669abcfa72d617aa355fa5941c
– 23c5e9fd621c7999727ce09fd152a2773bc350848aedba9c930f4ae2342e7d09
– 69570c69086e335f4b4b013216aab7729a9bad42a6ce3baecf2a872d18d23038

Malicious DLLs embedded in MSI font packages:
– b306264d6fc9ee22f3027fa287b5186cf34e7fb590d678ee05d1d0cff337ccbf

Coin miner malware:
– fcf64fc09fae0b0e1c01945176fce222be216844ede0e477b4053c9456ff023e (xbox-service.exe)
– 1d596d441e5046c87f2797e47aaa1b6e1ac0eabb63e119f7ffb32695c20c952b (pagefile.sys)

Software supply chain download server:

– hxxp://vps11240[.]hyperhost[.]name/escape/[some_font_package].msi (IP: 91[.]235 [.]129 [.]133)

Command-and-control/coin mining:
– hxxp://data28[.]somee [.]com/data32[.]zip
– hxxp://carma666[.]byethost12 [.]com/32[.]html
