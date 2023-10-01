# OpenVAS
Using OpenVAS vulnerability managements to remediate vulnerabilities

<h2>Introduction</h2>

<h2>Initial Scan</h2>
In the initial uncredentialed scan we can see the system contains three vulnerabilities ranging from medium to low. Upon closer inspection these vulnerabilities are Distributed computing environment / Remote procedure calls, Depreciated TLSv1.0 and TLSv1.1, and ICMP Timestamp reply information disclosure. This scan does not show as much as it is uncredentialed and will not give a greater depth as the other scans will, below the scans will go into more detail as credentials are beginning to be added into the OpenVAS scanner.
<br>Vulnerabilities: 33</br>
<br>Severity: 5.00</br>
<br>CVEs: 2</br>

<h2>Credentialed Scan</h2>
The first credentialed scan is where we can really start having an insight into how vulnerable this system truly is. The scan report shows multiple severity 10 vulnerabilities, mainly consisting of problems from Adobe Reader, Firefox, VLC player, and outdated windows versions. As we can see down below the drastic increases in all categories highlights how important credentialed scans are and how much more probing these types of scans can do.
<br>Vulnerabilities: 139</br>
<br>Severity: 10.00</br>
<br>CVEs: 82</br>

<h2>Remediation 1 Outdated software</h2>

<br>Vulnerabilities: 56</br>
<br>Severity: 7.8</br>
<br>CVEs: 4</br>

<h2>Remediation 2 OS updates</h2>

<br>Vulnerabilities: 52</br>
<br>Severity: 5.00</br>
<br>CVEs: 2</br>

<h2>Remediation 3 Remainder</h2>

<br>Vulnerabilities: 37</br>
<br>Severity: 0(Log)</br>
<br>CVEs: 0</br>

<h2>Scan Results</h2>
<b>Overview of scan results</b>

<img width="959" alt="Scan Results" src="https://github.com/ChrisHaugaard/OpenVAS/assets/140214520/f3d45d25-07e4-4cd6-a6af-550abc1bc8d6">

Incrimentally as more safety mesaures and remediations are applied, the overall severity of the system goes down. With the initial credentialed scan consisting of a severity score of 10.0 going down to 0 (only log alerts) as we apply the last recommended security improvements. 
<br></br>



<h2>Conclusion</h2>
