# Zlux App Server Changelog

All notable changes to the Zlux App Server package will be documented in this file.

## v2.11.0

- Bugfix: The server couldn't load more than one certificate authority specified within the zowe.certificate.pem.certificateAuthorities section under any condition. Now, it is supported regardless of if the section is an array or a comma-separated string. (#266)

## v2.10.0

- Enhancement: Migrated app-server configuration options into a "defaults.yaml" file which adheres to the schema of the Zowe config. This allows users to see the default behaviors more clearly, and can serve as an example by which users can customize their Zowe config to override such defaults. (#247)
- Bugfix: Fixed the URLs app-server would print in the logs describing where it was accessible from. Messages were incorrectly pointing at the discovery server instead of the gateway server. (#247)
CHANGELOG: Update blank.yml
