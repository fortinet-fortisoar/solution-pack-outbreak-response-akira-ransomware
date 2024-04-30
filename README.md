# Release Information 

- **Version**: 1.0.0 
- **Certified**: No 
- **Publisher**: Fortinet 
- **Compatible Version**: FortiSOAR 7.4.0 and later 

# Overview 

FortiGuard Labs continue to observe detections in the wild related to the Akira ransomware group. According to the new report by CISA it has targeted over 250 organizations since the past year, affecting numerous businesses and critical infrastructure entities across North America, Europe, and Australia. The gang has made over $42 million from the attacks as ransom payments.  

 The **Outbreak Response - Akira Ransomware** solution pack works with the Threat Hunt rules in [Outbreak Response Framework](https://github.com/fortinet-fortisoar/solution-pack-outbreak-response-framework/blob/release/1.1.0/README.md#threat-hunt-rules) solution pack to conduct hunts that identify and help investigate potential Indicators of Compromise (IOCs) associated with this vulnerability within operational environments of *FortiSIEM*, *FortiAnalyzer*, *QRadar*, *Splunk*, and *Azure Log Analytics*.

 The [FortiGuard Outbreak Page](https://www.fortiguard.com/outbreak-alert/akira-ransomware) contains information about the outbreak alert **Outbreak Response - Akira Ransomware**. 

## Background: 

First detected in March/April of 2023, this ransomware group primarily focuses on small to medium-sized businesses, driven by financial motives. Like other notorious ransomware, Akira utilizes familiar tactics such as Ransomware-as-a-Service and double extortion to maximize their profits. 

The ransomware uses virtual private network (VPN) service without multifactor authentication (MFA)- mostly using known Cisco vulnerabilities CVE-2020-3259 and CVE-2023-20269, external-facing services such as Remote Desktop Protocol, spear phishing, and the abuse of valid credentials. 

These credentials are typically acquired through brute force attacks or obtained from the dark web. Once inside, threat actors deploy various tools and malware to conduct reconnaissance, dump credentials, exfiltrate data, and move laterally within the network.

Initial iterations of the Akira ransomware variant were coded in C++ and encrypted files with a .akira extension. However, from August 2023 onwards, certain Akira attacks transitioned to utilizing Megazord, featuring Rust-based code that encrypts files with a .powerranges extension. Akira threat actors persist in employing both Megazord and Akira, including the newer version, Akira_v2. 

## Announced: 

Fortinet has existing AV signatures and behaviour-based detections to detect and block Akira Ransomware, however it is always recommended to follow best practices and apply relavant patches to mitigate threat and reduce the likelihood/impact of ransomware incidents.
https://www.fortinet.com/resources/cyberglossary/how-to-prevent-ransomware
 

## Latest Developments: 

April 19, 2024: FortiGuard Labs released a Threat Signal.
https://www.fortiguard.com/threat-signal-report/5426 

April 18, 2024: The United States’ Federal Bureau of Investigation (FBI), Cybersecurity and Infrastructure Security Agency (CISA), Europol’s European Cybercrime Centre (EC3), and the Netherlands’ National Cyber Security Centre (NCSC-NL) are releasing this joint cyber security advisory (CSA):https://www.cisa.gov/news-events/cybersecurity-advisories/aa24-109a

Feb 15, 2024: CISA added (CVE-2020-3259) Cisco ASA and FTD Information Disclosure Vulnerability to known exploited vulnerabilties catalog. 

October 12, 2023: Fortinet released a detailed blog on Akira Ransomware
https://www.fortinet.com/blog/threat-research/ransomware-roundup-akira

Sep 13, 2023: CISA added (CVE-2023-20269): Cisco Adaptive Security Appliance and Firepower Threat Defense Unauthorized Access Vulnerability to its known exploited vulnerabilties catalog. 

# Next Steps
 | [Installation](./docs/setup.md#installation) | [Configuration](./docs/setup.md#configuration) | [Usage](./docs/usage.md) | [Contents](./docs/contents.md) | 
 |--------------------------------------------|----------------------------------------------|------------------------|------------------------------|