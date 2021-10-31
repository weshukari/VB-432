# Disclosure Discovery

Every project MUST provide a link to its security vulnerability database in an obvious place. Ideally this should be on the root page of the main domain of the given project.
This MAY be a sub-domain in case it is a sub-project of a larger initiative. If the project has a dedicated page for its disclosure process discovery then this is also considered
a good place for this link. The link MAY use the custom link relation php-vuln-disclosures, ie. for example `<link rel="php-vuln-disclosures" href="http://example.org/disclosures"/>`.

In addition the following tags are added:
* reported (initial report date)
* reportedBy (contact information for the persons or entity that initially reported the vulnerability)
* resolvedBy (contact information for the persons or entity that resolved the vulnerability)
* name (name of the product, MUST)
* cve (unique CVE ID)
* cwe (unique CWE ID)
* severity (low, medium high)
* affected (version(s) using composer syntax [5])
* status (open, in progress, disputed, completed, MUST)
* remediation (textual description for how to fix an affected system)
* remediationType (workaround, mitigation, vendor fix, none available, will not fix)
* remediationLink (URL to give additional information for remediation)

https://tools.ietf.org/html/rfc4287
