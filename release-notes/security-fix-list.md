# Security Fixes Summary

The following is a list of tracked _**C**ommon **V**ulnerabilities and **E**xposures_ that have been reported and analyzed, which can or have impacted Payara Server across releases:

| ID | Status | Summary | Observations |
| :--- | :--- | :--- | :--- |
| [CVE-2007-6726](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2007-6726) | FIXED | XSS Vulnerabilities in **Dojo** libraries used for admin console | Since 4.1.1.163 |
| [CVE-2012-2098](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2012-2098) | FIXED | Apache Commons Compress **bzip2** vulnerability allows DDoS attacks | Since 4.1.1.163 |
| [CVE-2013-2035](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2013-2035) | FIXED | Race condition in outdated **jLine** code allows arbitrary code execution | Since 4.1.1.171 |
| [CVE-2014-0050](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-0050) | FIXED | Apache Commons FileUpload allows DDoS attacks via crafted `Content-Type` headers | Since 4.1.1.154.1 |
| [CVE-2015-0254](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-0254) | N/A | Vulnerabilities on Apache JSTL allows arbitrary code injection | Payara Server uses the `FEATURE_SECURE_PROCESSING` feature of JAXP so is not affected |
| [CVE-2015-3237](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-3237) | N/A | Vulnerabilities in smb\_request\_state function in **cURL** | Payara Server doesn't ship with either **cURL** or **licurl** so it's not affected |
| [CVE-2015-5346](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5346) | N/A | Apache Tomcat Vulnerability in session recycling for **SSL **requests | Payara Server implementation of the Request class doesn't contain the problematic variable being recycled |
| [CVE-2015-5351](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5351) | N/A | Apache Tomcat Manager Applications Session and **CSRF **token vulnerabilities | Unrelated to Payara Server since this affects specific Tomcat applications |
| [CVE-2016-0706](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-0706) | N/A | Apache Tomcat Vulnerability on `StatusManagerServlet` component allows reads of HTTP requests and discover session IDs | Payara Server doesn't use the `StatusManagerServlet` component so it's not affected |
| [CVE-2016-0714](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-0714) | N/A | Session persistence in Apache Tomcat allows arbitrary code injection | Payara Server doesn't use the affected objects in the same way that Tomcat does so the flaw is not present |
| [CVE-2016-0763](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-0763) | FIXED | Vulnerability in `ResourceLinkFactory.setGlobalContext` method on Apache Tomcat | Since 4.1.1.164.1 |
| [CVE-2016-3092](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-3092) | FIXED | Apache Commons FileUpload allows DDoS attacks via `Multipart` class | Since 4.1.1.163 |
| [CVE-2016-3427](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-3427) | FIXED | Unspecified vulnerability in various versions of the Oracle JDK and JRockit | Since 4.1.1.164.1 |
| [CVE-2016-3607](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-3607) | FIXED | Unspecified vulnerability on Oracle GlassFish 3.0+ affects confidentiality | Since 4.1.1.163 |
| [CVE-2016-3608](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-3608) | N/A | Unspecified vulnerability on Oracle GlassFish 3.0.1 affects confidentiality | Affects an older version of GlassFish but not Payara Server |
| [CVE-2016-5388](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-5388) | FIXED | Apache Tomcat does not protect applications from untrusted data when using the CGI Servlet | Since 4.1.1.163.1 |
| [CVE-2016-5477](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-5477) | N/A | Unspecified vulnerability on Oracle GlassFish 3.0.1 affects confidentiality | Affects an older version of GlassFish but not Payara Server |
| [CVE-2016-5519](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-5519) | PENDING | Unspecified vulnerability on JSF implementation for Oracle Glassfish 3.0+ | Pending for assesment |
| [CVE-2016-6816](http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-6816) | N/A | Apache Tomcat HTTP request parsing vulnerability allow injection of data into reponse | Payara Server doesn't have included the Coyote components affected |


