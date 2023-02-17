# Fase 3. Vakliteratuur raadplegen - nota's

## JabRef

De belangrijkste bronnen worden in het JabRef document gezet zodat we deze kunnen verwerken/citen wanneer we hierover een stukje gaan schijven.

## Linken volgens Onderzoek en MINDMAP

### Wat is Apache log4j?

- Apache Software foundation: <https://www.apache.org/>
- <https://logging.apache.org/log4j/2.x/>
- log4j 2.0: <https://grobmeier.solutions/the-new-log4j-2-0-05122012.html>
- <https://www.ralphgoers.com/post/why-was-log4j-2-created>
- end-of-live (v1.2): <https://logging.apache.org/log4j/2.x/index.html#News>
- welkome log4j 2: <https://logging.apache.org/log4j/2.x/manual/index.html>
- async: <https://logging.apache.org/log4j/2.x/manual/async.html#Performance>
- log levels: <https://logging.apache.org/log4j/2.x/manual/customloglevels.html>
- architctuur: <https://logging.apache.org/log4j/2.x/manual/architecture.html>
- config: <https://logging.apache.org/log4j/2.x/manual/configuration.html>
- class: <https://logging.apache.org/log4j/1.2/apidocs/org/apache/log4j/Level.html#TRACE>
- random access file: <https://docs.oracle.com/javase/7/docs/api/java/io/RandomAccessFile.html>
- layouts: <https://logging.apache.org/log4j/2.x/manual/layouts.html>
- Graylog Extended Log Format - events: <https://archivedocs.graylog.org/en/2.0/pages/gelf.html>
- syslog <https://datatracker.ietf.org/doc/html/rfc5424>
- filters <https://logging.apache.org/log4j/2.x/manual/filters.html>
- Class TTCCLayout: <https://logging.apache.org/log4j/1.2/apidocs/org/apache/log4j/TTCCLayout.html>
- Class NDC: <https://people.apache.org/~carnold/log4j/docs/org/apache/log4j/NDC.html>
- Class MDC: <https://logging.apache.org/log4j/1.2/apidocs/org/apache/log4j/MDC.html>

#### Versies

- <https://logging.apache.org/log4j/1.2/changes-report.html>
- <https://lists.apache.org/thread/pwx9zs967yk7zsv7nlmv7nhwkc359k2m>
- <https://logging.apache.org/log4j/2.x/changes-report.html>

### Wat is de log4 kwetsbaarheid?

- <https://www.comptia.org/blog/log4j-vulnerability>
- <https://arstechnica.com/information-technology/2021/12/minecraft-and-other-apps-face-serious-threat-from-new-code-execution-bug/>
- <https://www.cyberkendra.com/2021/12/worst-log4j-rce-zeroday-dropped-on.html>
- fork from ori creator v1.2.17: <https://reload4j.qos.ch/>
- <https://www.theguardian.com/technology/2021/dec/10/software-flaw-most-critical-vulnerability-log-4-shell>
- <https://www.wsj.com/articles/what-is-the-log4j-vulnerability-11639446180>
- wat en fix: <https://nakedsecurity.sophos.com/2021/12/13/log4shell-explained-how-it-works-why-you-need-to-know-and-how-to-fix-it/>
- <https://blog.cloudflare.com/inside-the-log4j2-vulnerability-cve-2021-44228/>
- CISA director statement: <https://www.cisa.gov/news/2021/12/11/statement-cisa-director-easterly-log4j-vulnerability>
- FTC (Fedaral Trade Commision) statement: <https://www.ftc.gov/policy/advocacy-research/tech-at-ftc/2022/01/ftc-warns-companies-remediate-log4j-security-vulnerability>
- <https://www.wsj.com/articles/what-is-the-log4j-vulnerability-11639446180>

### Wat is Log4Shell (CVE-2021-44228)?

- <https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-44228>
- <https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-45046>
- <https://nvd.nist.gov/vuln/detail/CVE-2021-45105>
- <https://nvd.nist.gov/vuln/detail/CVE-2021-44832>
- <https://github.com/advisories/GHSA-jfh8-c2jp-5v3q>
- <https://www.mcafee.com/blogs/enterprise/mcafee-enterprise-atr/log4shell-vulnerability-is-the-coal-in-our-stocking-for-2021/>
- Goede uitleg + img van Bitdefender: <https://businessinsights.bitdefender.com/technical-advisory-zero-day-critical-vulnerability-in-log4j2-exploited-in-the-wild>
- Goede uitleg van Rapid7: <https://www.rapid7.com/blog/post/2021/12/10/widespread-exploitation-of-critical-remote-code-execution-in-apache-log4j/>
- Goede afbeeldingen van Juniper networks: <https://blogs.juniper.net/en-us/security/apache-log4j-vulnerability-cve-2021-44228-raises-widespread-concerns>
- cloudflare blog: <https://blog.cloudflare.com/inside-the-log4j2-vulnerability-cve-2021-44228/>
- <https://www.lunasec.io/docs/blog/log4j-zero-day/>
- <https://arstechnica.com/information-technology/2021/12/the-critical-log4shell-zero-day-affects-a-whos-who-of-big-cloud-services/>
- <https://www.washingtonpost.com/technology/2021/12/20/log4j-hack-vulnerability-java/>
- <https://www.trendmicro.com/en_us/research/21/l/patch-now-apache-log4j-vulnerability-called-log4shell-being-acti.html>
- situatie via blog (podcast): <https://danielmiessler.com/podcast/news-analysis-no-311/>
- Goede uitleg + img: <https://jfrog.com/blog/log4shell-0-day-vulnerability-all-you-need-to-know/>

### Wie is er getroffen? (enkele voorbeelden)

- Defensie België: <https://archive.ph/rJv36>
- Attack surface (risk based security): <https://www.riskbasedsecurity.com/2021/12/14/log4shell-log4j-vulnerability-attack-surface-variant-and-remediation/>
- blog Apache met getroffen partijen: <https://blogs.apache.org/security/entry/cve-2021-44228>
- Minecraft: <https://help.minecraft.net/hc/en-us/articles/4416199399693-Security-Vulnerability-in-Minecraft-Java-Edition>
- Amazon: <https://aws.amazon.com/security/security-bulletins/AWS-2021-006/>
- <https://www.pcmag.com/news/countless-serves-are-vulnerable-to-apache-log4j-zero-day-exploit>
- Apple iCloud: <https://9to5mac.com/2021/12/14/apple-patches-log4shell-icloud-vulnerability/>
- Harder voor kleine bedrijven om te verdedigen + interview: <https://eu.usatoday.com/story/money/business/2021/12/16/log-4-j-vulnerability-small-business/8910567002/>
- National security issue - meeting White House: <https://gizmodo.com/after-log4j-open-source-software-is-now-a-national-sec-1848356403>
- White House: <https://www.zdnet.com/article/after-log4j-white-house-worries-about-the-next-big-open-source-flaw/>
- BSI met reportage: <https://www.tagesschau.de/inland/bsi-schadsoftware-101.html>
- BSI official statement: <https://www.bsi.bund.de/DE/Service-Navi/Presse/Pressemitteilungen/Presse2021/211211_log4Shell_WarnstufeRot.html>
- Overheidswebsites Quebec: <https://www.cbc.ca/news/canada/montreal/quebec-cybersecurity-threat-government-website-1.6283133>
- Alibaba Cloud: <https://www.scmp.com/tech/big-tech/article/3160670/apache-log4j-bug-chinas-industry-ministry-pulls-support-alibaba-cloud>
- Microsoft: <https://www.zdnet.com/article/log4j-flaw-attacks-are-causing-lots-of-problems-microsoft-warns/>
- SAP: <https://www.itsecuritynews.info/sap-patches-log4shell-vulnerability-in-more-applications/>
- Wereldwijd: <https://www.bostonglobe.com/2021/12/15/business/emerging-log4j-software-bug-spawns-worldwide-worry-over-cyber-attacks/>

### Hoe zit de anatomie van de aanval in elkaar? (Log4j + JNDI vulnerability)

Zie ook vorige artikels met goede uitleg en afbeeldingen als omschrijving

#### Java

- <https://www.oracle.com/java/technologies/javase/8u121-relnotes.html>

#### jndi

- <https://www.veracode.com/blog/research/exploiting-jndi-injections-java>
- lookups: <https://logging.apache.org/log4j/2.x/manual/lookups.html>

### Hoe kan ik getroffen pakketten identificeren?

- <https://www.tahawultech.com/news/qualys-offers-free-access-to-its-web-application-scanning-app-to-help-organizations-quickly-find-log4shell-vulnerabilities/>
- Linkedin bijdrage door Douglas Everson (vid en workshop): <https://www.linkedin.com/posts/douglaseverson_recording-and-post-production-wrapped-presentation-activity-6923252337415241728-Z8r1>
- Github en webap testing tools: CVE-2021-44228 [URL](https://log4shell.tools/) and [gitRepo](https://github.com/)

### Hoe kan ik de Log4Shell kwetsbaarheid bestrijden en tegengaan?

- <https://issues.apache.org/jira/browse/LOG4J2-3201>
- <https://www.cisa.gov/news/2021/12/11/statement-cisa-director-easterly-log4j-vulnerability>
- Interessante gids: <https://www.lunasec.io/docs/blog/log4j-zero-day-mitigation-guide/>
- te volgen stappen: <https://thenewstack.io/log4shell-we-are-in-so-much-trouble/>
- Limit the protocols JNDI can use and restrict LDAP: <https://issues.apache.org/jira/browse/LOG4J2-3201>
- helpnetsecurity + img: <https://www.helpnetsecurity.com/2021/12/13/log4shell-update-cve-2021-44228/>

### Evolutie toestand log4j kwetsbaarheid en wat is er allemaal veranderd?

- Gebruiken: Kwetsbaarheid was eerder ontdek: <https://www.bloomberg.com/news/articles/2021-12-13/how-apache-raced-to-fix-a-potentially-disastrous-software-flaw>
- <https://www.wired.com/story/log4j-flaw-hacking-internet/>

#### inter

- <https://www.wiz.io/blog/10-days-later-enterprises-halfway-through-patching-log4shell/>

#### post

- <https://logging.apache.org/log4j/2.x/security.html>
- mitigation - Cloudflare: <https://blog.cloudflare.com/cve-2021-44228-log4j-rce-0-day-mitigation/>
- <https://cyber.gc.ca/en/news/statement-minister-national-defence-apache-vulnerability>
- LOG4J2-3198: Log4j2 no longer formats lookups in messages by default: <https://github.com/apache/logging-log4j2/commit/001aaada7dab82c3c09cde5f8e14245dc9d8b454>
- patch: <https://www.zdnet.com/article/second-log4j-vulnerability-found-apache-log4j-2-16-0-released/>
- end-of-live (v1.2): <https://logging.apache.org/log4j/2.x/index.html#News>
- welkome log4j 2: <https://logging.apache.org/log4j/2.x/manual/index.html>
- hardening: <https://reload4j.qos.ch/>
- recommended upgrades: <https://blogs.apache.org/foundation/entry/apache_logging_services_project_announces>
- Restrict LDAP access via JNDI: <https://github.com/apache/logging-log4j2/pull/608>
- Disable JNDI by default: <https://issues.apache.org/jira/browse/LOG4J2-3208>
- Remove support for Lookups in messages: <https://issues.apache.org/jira/browse/LOG4J2-3211>
- Minecraft patched - single vs multiplayer<https://www.minecraft.net/en-us/article/important-message--security-vulnerability-java-edition>

### Proof-of-Concept (PoC)

- <https://www.tenable.com/blog/cve-2021-44228-proof-of-concept-for-critical-apache-log4j-remote-code-execution-vulnerability>
- <https://thesecmaster.com/how-does-the-log4j-vulnerability-work-in-practical/>

#### Gebruikt voor eigen PoC

- automated environment using ansible with a [vagrant skeleton](https://github.com/bertvv/ansible-skeleton) built by bertvv
- log4j CVE-2021-44228 poc [githubRepo](https://github.com/kozmer/log4j-shell-poc) built by kozer
- log4j CVE-2021-44228 testing tools [URL](https://log4shell.tools/) and [gitRepo](https://github.com/alexbakker/log4shell-tools) built by Alexander Bakker

## Per Categorie

### Repo

- Nationaal Cyber Security Centrum (NCSC-NL): Log4shell vulnerabilities (CVE-2021-44228, CVE-2021-45046, CVE-2021-4104, CVE-2021-45105): <https://github.com/NCSC-NL/log4shell>
- snyk-labs - Awesome Log4Shell: <https://github.com/snyk-labs/awesome-log4shell>

### Cijfers/in kaart

- Hackers launch more than 1.2m attacks through Log4J flaw: <https://www.ft.com/content/d3c244f2-eaba-4c46-9a51-b28fc13d9551>
- Checkpoint Goede cijfers en img: <https://blog.checkpoint.com/2021/12/13/the-numbers-behind-a-cyber-pandemic-detailed-dive/>
- <https://blog.sonatype.com/why-did-log4shell-set-the-internet-on-fire>
- <https://security.googleblog.com/2021/12/understanding-impact-of-apache-log4j.html>
- <https://crowdsec.net/log4j-tracker/>
- <https://cve.report/CVE-2021-44228>
- targeting in cijfers: <https://www.computerweekly.com/news/252510939/Almost-half-of-networks-probed-for-Log4Shell-weaknesses>

#### Use cases voor black hats

- crypomining/ spionnage: <https://www.wired.com/story/log4j-log4shell-vulnerability-ransomware-second-wave/>
- ransomware: <https://arstechnica.com/information-technology/2021/12/as-log4shell-wreaks-havoc-payroll-service-reports-ransomware-attack/>
- botnets: <https://www.zdnet.com/article/log4j-rce-activity-began-on-december-1-as-botnets-start-using-vulnerability/>

### Recent

- <https://www.ibm.com/blogs/psirt/security-bulletin-vulnerability-in-apache-log4j-affects-ibm-elastic-storage-system-cve-2021-4104/>
- <https://jfrog.com/log4j-log4shell-resources/>
- <https://javarepos.com/lib/apache-logging-log4j2-java-logging>
- <https://www.darkreading.com/vulnerabilities-threats/three-months-later-41-of-log4j-downloads-are-of-vulnerable-versions>

### Ebook

- <https://www.idgconnect.com/resources/232146/new-security-and-risk-management-in-the-wake-of-the-log4j-vulnerability>

### Scolar

- article: The Race to the Vulnerable: Measuring the Log4j Shell Incident: <https://arxiv.org/abs/2205.02544>
- article: On FICO-Like Vulnerability Rating of Source Code
  - <https://www.researchgate.net/publication/360074800_On_FICO-Like_Vulnerability_Rating_of_Source_Code>
  - <https://www.researchgate.net/profile/Joseph-Barr/publication/360074800_On_FICO-Like_Vulnerability_Rating_of_Source_Code/links/62604691bca601538b5a339c/On-FICO-Like-Vulnerability-Rating-of-Source-Code.pdf>
- article: The Dangerous Combo: Fileless Malware and Cryptojacking
  - <https://ieeexplore.ieee.org/abstract/document/9764043>
- paper: Redefining the Web Attack Surface:
  - <https://www.ndss-symposium.org/wp-content/uploads/madweb2022_23010_paper.pdf>
  - <https://www.ndss-symposium.org/ndss-paper/auto-draft-277/>
- inproceedings: Deceptive directories and "vulnerable" logs: a honeypot study of the LDAP and log4j attack landscape
  - <https://www.researchgate.net/publication/360015240_Deceptive_directories_and_vulnerable_logs_a_honeypot_study_of_the_LDAP_and_log4j_attack_landscape>
  - <https://www.researchgate.net/profile/Emmanouil-Vasilomanolakis/publication/360015240_Deceptive_directories_and_vulnerable_logs_a_honeypot_study_of_the_LDAP_and_log4j_attack_landscape/links/625d32f69be52845a90c238c/Deceptive-directories-and-vulnerable-logs-a-honeypot-study-of-the-LDAP-and-log4j-attack-landscape.pdf>
- thesis: Constructing a vulnerability knowledge graph
  - <https://nmbu.brage.unit.no/nmbu-xmlui/handle/11250/2995275>
  - <https://nmbu.brage.unit.no/nmbu-xmlui/bitstream/handle/11250/2995275/thesis.pdf?sequence=1&isAllowed=y>

### Software repo

- <https://repo1.maven.org/maven2/org/apache/logging/log4j/log4j-core/>
- <https://www.oracle.com/java/technologies/javase/javase8-archive-downloads.html>

### Audit reports

- <https://www.nist.gov/itl/smallbusinesscyber/nist-cybersecurity-framework>
- <https://www.offensive-security.com/reports/sample-penetration-testing-report.pdf>
- <https://www.nist.gov/itl/smallbusinesscyber/planning-guides/planning-tools-workbooks>
- <https://www.nist.gov/itl/smallbusinesscyber/planning-guides/nist-cybersecurity-framework>
- <https://www.nist.gov/industry-impacts/cybersecurity-framework>
- info: <https://www.appknox.com/blog/nist-cybersecurity-framework>