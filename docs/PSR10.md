## Introduction
***

There are two aspects with dealing with security issues: One is the process by which security issues are reported and fixed in projects, the other is how the general public is informed about the issues and any remedies available. While PSR-10 addresses the later, this PSR, ie. PSR-9, deals with the former. So the goal of PSR-9 is to define the process by which security researchers and report security vulnerabilities to projects. It is important that when security vulnerabilities are found that researchers have an easy channel to the projects in question allowing them to disclose the issue to a controlled group of people.

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in [Link](http://tools.ietf.org/html/rfc2119 "RFC 2119").

## Goal
***

The goal of this PSR is to give researchers, project leads, upstream project leads and end users a defined and structured process for disclosing security vulnerabilities.

## Security Disclosure Process Discovery
***

Every project MUST provide a link to its security disclosure process in an obvious place. Ideally this should be on the root page the main domain of the given project. This MAY be a sub-domain in case it is a sub-project of a larger initiative. The link MAY use the custom link relation `php-vuln-reporting`, ie. for example `<link rel="php-vuln-reporting" href="http://example.org/security"/>`.

Note that projects MAY not have a dedicated domain. For example a project hosted on Github, Bitbucket or other service should still ensure that the process is referenced on the landing page, ie. for example [](http://github.com/example/somelib) should ensure that the default branch has a README file which references the procedures used so that it is automatically displayed.

## Default Procedures
***

* `[project name]` denotes the name on which the project uses to identify itself.
* `[project domain]` denotes the main (sub)domain on which the project relies.
