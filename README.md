# DevSecOps v praxi s využitím Azure
Repozitář s osnovou, labs, návody a odkazy pro kurz [DevSecOps v praxi s využitím Azure](https://www.datascript.cz/kurzy/azure/devsecops-v-praxi-s-vyuzitim-azure/)

- [Teorie a info](#information)
  - [Network security](https://docs.microsoft.com/en-us/azure/security/fundamentals/network-best-practices) - (EN)
  - [Operation security checklist](https://docs.microsoft.com/en-us/azure/security/fundamentals/operational-checklist) - (EN)
  - [Web security checklist](security-checklist.md) - (EN)
  - [Prezentace](#presentations)
  - [Iniciativy](#Iniciativy)
  - [Staying up-to-date](#keeping-informed)
- [Kurz](#Kurz)
  - [Policy as code](#policy-as-code)
  - [IaC repozitář - RockPaperScissorsLizardSpock](https://github.com/zmaten/Uvod-do-DevSecOps-RockPaperScissorsLizardSpock)
  - [Nezabezpečené testovací aplikace](#Nezabezpečené-testovací-aplikace)
- [Nástroje](#Nástroje)
  - [Software bill of materials](#Generování-SBoM)
  - [Dashboardy](#Dashboardy)
  - [Automatizace](#Automatizace)
  - [Analýza a vyhledávání chyb](#Analýza-a-vyhledávání-chyb)
  - [Testování](#Testování)
  - [Alerting](#alerting)
  - [Threat Intelligence](#threat-intelligence)
  - [Attack Modeling](#attack-modeling)
  - [Secret Management](#secret-management)
- [Ostatní](#Ostatní)
  - [Konference](#Konference)
  - [Podcasty](#Podcasty)
  - [Knihy](#Knihy)


## Iniciativy
V současné době probíhá řada iniciativ, jejichž cílem je přenést bezpečnost a dodržování předpisů do systému DevOps.

* [OWASP](https://owasp.org)
* [DevSecOps](http://devsecops.org)
* [OpenDevSecOps](https://opendevsecops.org)



# Kurz
Odkazy a repozitáře pro kurz

## Policy as Code
Repozitář pro trénink policy as code

 * [PaC repozitář](https://github.com/Azure/manage-azure-policy/blob/main/tutorial/azure-policy-as-code.md)
 *
## IaC
Repozitář pro trénink infrastructure as code

 * [IaC repozitář - RockPaperScissorsLizardSpock](https://github.com/zmaten/Uvod-do-DevSecOps-RockPaperScissorsLizardSpock)

## Nezabezpečené testovací aplikace
Důležité je prohloubit si znalosti tím, že se naučíte, jak prolomit aplikace, které jsou zranitelné kvůli chybám v zabezpečení.  Tato část obsahuje seznam zranitelných aplikací, které lze nasadit, abyste se naučili, co nedělat.  Stejné aplikace lze zabezpečit odstraněním záměrných zranitelností, abyste se naučili, jak zabránit útočníkům v přístupu k základní infrastruktuře nebo datům.

* [NodeGoat](https://github.com/owasp/nodegoat) (Node)
* [OWASP Juice Shop](https://github.com/OWASP/glue) (NodeJS/Angular)
* [WebGoat](https://github.com/WebGoat/WebGoat) (Web App)
* [WebGoat.Net](https://github.com/OWASP/WebGoat.NET) (.NET)


# Nástroje
Užitečné nástroje pro budování platformy DevSecOps. Členěno podle kategorií (neomezuje se na Azure/MS)

## Generování SBoM
* [CycloneDX](https://cyclonedx.org/) (Info)
* [CycloneDX - GitHub](https://github.com/CycloneDX/cyclonedx-dotnet) (.NET)

## Dashboardy

* [Grafana](http://grafana.org/)
* [Kibana](https://www.elastic.co/products/kibana)

## Automatizace

* [Demisto](https://www.demisto.com/community/)
* [OWASP Glue](https://github.com/OWASP/glue)
* [StackStorm](https://github.com/StackStorm/st2)
* [Insider CLI](https://github.com/insidersec/insider)

## Analýza a vyhledávání chyb
Tento seznam nástrojů poskytuje možnosti potřebné pro vyhledávání bezpečnostních anomálií a identifikaci pravidel, která by měla být automatizována a rozšířena tak, aby podporovala požadavky na rozsah.

* [GRR](https://github.com/google/grr)
* [kube-hunter](https://github.com/aquasecurity/kube-hunter)
* [mig](https://github.com/mozilla/mig)
* [Mirador](http://fathom.info/mirador/)
* [moloch](https://github.com/aol/moloch)
* [MozDef](https://github.com/mozilla/MozDef)
* [osquery](https://osquery.io/)
* [OSSEC](http://ossec.github.io/)
* [osxcollector](https://github.com/Yelp/osxcollector)


## Testování
Testing is an essential element of a DevSecOps program because it helps to prepare teams for Rugged operations and to determine security defects before they can be exploited.

* [Checkov](https://github.com/bridgecrewio/checkov/)
* [Deepfence ThreatMapper](https://github.com/deepfence/ThreatMapper)
* [HusckyCI](https://github.com/globocom/huskyci)
* [IronWASP](https://ironwasp.org/)
* [kube-bench](https://github.com/aquasecurity/kube-bench)
* [microscanner](https://github.com/aquasecurity/microscanner)
* [Node Security Platform](https://nodesecurity.io/)
* [npm-check](https://www.npmjs.com/package/npm-check)
* [npm-outdated](https://docs.npmjs.com/cli/outdated)
* [OSS Fuzz](https://github.com/google/oss-fuzz)
* [OWASP OWTF](https://www.owasp.org/index.php/OWASP_OWTF)
* [OWASP ZAP](https://www.owasp.org/index.php/OWASP_Zed_Attack_Proxy_Project)
* [OWASP ZAP Node API](https://github.com/zaproxy/zap-api-nodejs)
* [Progpilot](https://github.com/designsecurity/progpilot)
* [PureSec (Serverless Security)](https://www.puresec.io/)
* [RetireJS](https://github.com/RetireJS/retire.js)


## Alerting
Doba odezvy je kritická a zásadní pro reakci na incident, která je nutná k nápravě bezpečnostní závady. Tyto odkazy obsahují některé z projektů, které zajišťují alerting a notifikace.
* [411](https://github.com/kiwiz/411)
* [Alerta](https://github.com/guardian/alerta)
* [Elastalert](https://github.com/yelp/elastalert)
* [MozDef](https://github.com/mozilla/MozDef)

## Threat Intelligence
Tato kategorie obsahuje nástroje, které jsou užitečné pro zachycení informací o hrozbách a jejich shromažďování.
* [Alien Vault OTX](https://otx.alienvault.com/)
* [Critical Stack](https://intel.criticalstack.com)
* [IBM X-Force](https://exchange.xforce.ibmcloud.com)
* [IntelMQ Feeds](https://github.com/certtools/intelmq-feeds-documentation)
* [OpenTPX](https://www.opentpx.org)
* [Passive Total](https://www.passivetotal.org)
* [STIX, TAXII](https://oasis-open.github.io/cti-documentation/)
* [Threat Connect](https://threatconnect.com/)

## Attack Modeling

* [CAPEC](https://capec.mitre.org)
* [IriusRisk](https://www.continuumsecurity.net/threat-modeling-tool/)
* [Larry Osterman's Threat Modeling](https://blogs.msdn.microsoft.com/larryosterman/2007/10/01/some-final-thoughts-on-threat-modeling/)
* [SDL Threat Modeling Tool](https://www.microsoft.com/en-us/sdl/adopt/threatmodeling.aspx)
* [SeaSponge](http://mozilla.github.io/seasponge/)
* [Threat Risk Modeling](https://www.owasp.org/index.php/Threat_Risk_Modeling)

## Secret Management
Pro podporu security-as-code je třeba spravovat, zabezpečovat, udržovat a rotovat citlivá pověření a tajemství pomocí automatizace.  Níže uvedené projekty poskytují několik dobrých možností zabezpečení citlivých údajů používaných pro full-stack build a deployment.

* [BlackBox](https://github.com/StackExchange/blackbox)
* [Conjur](https://github.com/cyberark/conjur)
* [CredStash](https://github.com/fugue/credstash)
* [Git Secrets](https://github.com/awslabs/git-secrets)
* [Keybase](https://keybase.io)
* [Sops](https://github.com/mozilla/sops)
* [Transcrypt](https://github.com/elasticdog/transcrypt)
* [Vault](https://www.hashicorp.com/blog/vault.html)


# Ostatní
Užitečné odkazy pro použití mimo kurz
## Konference

* [DevSecCon](http://devseccon.com)
* [DevOps Connect](http://www.devopsconnect.com/)
* [DevOps Days](http://www.devopsdays.org/)
* [Goto Conference](http://gotocon.com)
* [IP Expo](http://www.ipexpoeurope.com/)
* [ISACA Ireland](http://www.isaca.org/chapters5/Ireland/conference/pages/Agenda.aspx)
* [RSA Conference](http://www.rsaconference.com)
* [All Day DevOps](https://www.alldaydevops.com/)

## Podcasty

* [Arrested DevOps](https://www.arresteddevops.com/)
* [Brakeing Down Security Podcast](http://www.brakeingsecurity.com/)
* [Darknet Diaries](https://darknetdiaries.com)
* [Defensive Security Podcast](http://www.defensivesecurity.org/)
* [DevOps Cafe](http://devopscafe.org/)
* [Down The Security Rabbithole](http://podcast.wh1t3rabbit.net/)
* [Food Fight Show](http://foodfightshow.org/)
* [OWASP 24/7](https://www.owasp.org/index.php/OWASP_Podcast)
* [Risky Business](http://risky.biz/)
* [Social Engineering Podcast](http://www.social-engineer.org/category/podcast/)
* [Software Engineering Radio](http://www.se-radio.net/team/kim-carter/)
* [Take 1 Security Podcast](https://danielmiessler.com/podcast/)
* [Tenable Security Podcast](http://www.tenable.com/podcast)
* [The Secure Developer](http://www.heavybit.com/library/podcasts/the-secure-developer/)
* [Trusted Sec Podcast](https://www.trustedsec.com/podcast/)

## Knihy
Anglicky psané knihy zaměřené na DevSecOps.

* [DevOpsSec](http://www.oreilly.com/webops-perf/free/devopssec.csp)
* [Docker Securitiy - Quick Reference](https://binarymist.io/publication/docker-security/)
* [Holistic Info-Sec for Web Developers](https://leanpub.com/b/holisticinfosecforwebdevelopers)
* [Securing DevOps](https://securing-devops.com/book)
* [The DevOps Handbook (Section VI)](https://www.oreilly.com/library/view/the-devops-handbook/9781457191381/)
