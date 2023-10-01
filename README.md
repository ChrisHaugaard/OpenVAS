# OpenVAS
Using OpenVAS vulnerability managements to remediate vulnerabilities

<h2>Introduction</h2>
In this lab, I will be exploring OpenVAS to view vulnerable systems with uncredentialed and credentialed scans with remediation happening in three separate remediation steps. This will include removal, updating, mitigation, and workarounds of vulnerabilities present on the computer over the five total scans. After the lab is done the computer will have been taken from a incredibly vulnerable security risk with a severity score of 10.00 to a computer with a severity score of 0.0(Log) with each step being documented.


<h2>Initial Scan</h2>
In the initial uncredentialed scan we can see the system contains three vulnerabilities ranging from medium to low. Upon closer inspection these vulnerabilities are Distributed computing environment / Remote procedure calls, Depreciated TLSv1.0 and TLSv1.1, and ICMP Timestamp reply information disclosure. This scan does not show as much as it is uncredentialed and will not give a greater depth as the other scans will, below the scans will go into more detail as credentials are beginning to be added into the OpenVAS scanner.
<br>Vulnerabilities: 33</br>
<br>Severity: 5.00</br>
<br>CVEs: 2</br>

<h2>Credentialed Scan</h2>
The first credentialed scan is where we can really start having an insight into how vulnerable this system truly is. The scan report shows multiple severity 10 vulnerabilities, mainly consisting of problems from Adobe Reader, Firefox, VLC player, and outdated windows versions. Firstly action will be taken against the outdated software by either removing or updating them. As we can see down below the drastic increases in all categories highlights how important credentialed scans are and how much more probing these types of scans can do.
<br>Vulnerabilities: 139</br>
<br>Severity: 10.00</br>
<br>CVEs: 82</br>

<h2>Remediation 1 Outdated software</h2>
In this scan report we can see the absence of VLC player, Adobe reader, and firefox as they have either been removed or updated to newer versions available. In this step actions were taken against IExpress and code execution over USB. For IExpress to be remediated I gave myself control of the file and removed it as there are two other browsers on the computer so it is considered not needed. No solution or patch has been made available for this type of vulnerability so since usb connections are not needed in this environment the decision to disable hidserv.dll was made. As the first remediation the same process of gaining priviledge over the file and disabling it occurred. The vulnerabilities have gone down significantly by over half now being removed by fixing outdated software that was present on the machine. As a result the computer is slowly becoming more secure as each remediation is applied.
<br>Vulnerabilities: 56</br>
<br>Severity: 7.8</br>
<br>CVEs: 4</br>

<h2>Remediation 2 OS updates</h2>
In this remediation step a simple search for os updates and application of optional os updates was applied to lower severity scores and increase security of the device.

<br>Vulnerabilities: 52</br>
<br>Severity: 5.00</br>
<br>CVEs: 2</br>

<h2>Remediation 3 Remainder</h2>
The remaining vulnerabilities that were chosen to be taken care of were Distributed computing environment / Remote procedure calls, Depreciated TLSv1.0 and TLSv1.1, and ICMP Timestamp reply information disclosure. Which is the same results from the initial uncredentialed report that was viewed in the beginning. For TLSv1.0 and TLSv1.1 the registry was edited to include that they will not be enabled and they will be disabled on startup. This will force the newer TLS protocols to be used instead. For ICMP reply information and DCE/RPC vulnerabilities the firewall was updated to not allow these types of traffic to occur. 

<br>Vulnerabilities: 37</br>
<br>Severity: 0(Log)</br>
<br>CVEs: 0</br>

<h2>Scan Results</h2>
<b>Overview of scan results</b>

<img width="959" alt="Scan Results" src="https://github.com/ChrisHaugaard/OpenVAS/assets/140214520/f3d45d25-07e4-4cd6-a6af-550abc1bc8d6">

Incrementally as more safety measures and remediations are applied, the overall severity of the system goes down. With the initial credentialed scan consisting of a severity score of 10.0 going down to 0 (only log alerts) as we apply the last recommended security improvements. For the ease of view in the lab these steps have been stretched out to highlight the different security solutions applied and created an easy to follow process of how the computer was secured.

<h2>Conclusion</h2>
We are now left with a computer that poses much less of a security risk to any connections it makes or organizations it is a part of by improving the security on the device. While there are still 37 Log severity alerts these are not substantial and the most they can give is information about the computer. While still useful and potentially a risk in its own right for the purpose of this lab they will be ignored as the lab was focusing on higher severity issues. The goal of this lab is now concluded as the computer that we began with now has no immediate high severity issues that need to be corrected.


