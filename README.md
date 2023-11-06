Templates are the core of [nuclei scanner](https://github.com/projectdiscovery/nuclei) which power the actual scanning engine. This repository stores and houses various templates for the scanner provided by our team as well as contributed by the community. We hope that you also contribute by sending templates via **pull requests** and grow the list.

<details>
<summary>Template Directory</summary>

```
├── LICENSE
├── README.md
├── basic-detections
│   ├── basic-xss-prober.yaml
│   └── general-tokens.yaml
├── brute-force
│   └── tomcat-manager-bruteforce.yaml

├── dns
│   ├── azure-takeover-detection.yaml
│   ├── cname-service-detector.yaml
│   ├── dead-host-with-cname.yaml
│   └── servfail-refused-hosts.yaml
├── files
│   ├── apc-info.yaml
│   ├── cgi-test-page.yaml
│   ├── debug-pprof.yaml
│   ├── dir-listing.yaml
│   ├── docker-registry.yaml
│   ├── drupal-install.yaml
│   ├── elasticsearch.yaml
│   ├── exposed-kibana.yaml
│   ├── exposed-svn.yaml
│   ├── filezilla.yaml
│   ├── firebase-detect.yaml
│   ├── git-config.yaml
│   ├── htaccess-config.yaml
│   ├── jkstatus-manager.yaml
│   ├── jolokia.yaml
│   ├── laravel-env.yaml
│   ├── lazy-file.yaml
│   ├── phpinfo.yaml
│   ├── public-tomcat-instance.yaml
│   ├── security.txt.yaml
│   ├── server-status-localhost.yaml
│   ├── telerik-dialoghandler-detect.yaml
│   ├── telerik-fileupload-detect.yaml
│   ├── tomcat-scripts.yaml
│   ├── wadl-files.yaml
│   ├── web-config.yaml
│   ├── wordpress-directory-listing.yaml
│   ├── wordpress-user-enumeration.yaml
│   ├── wp-xmlrpc.yaml
│   └── zip-backup-files.yaml
├── panels
│   ├── atlassian-crowd-panel.yaml
│   ├── cisco-asa-panel.yaml
│   ├── citrix-adc-gateway-detect.yaml
│   ├── compal.yaml
│   ├── crxde.yaml
│   ├── docker-api.yaml
│   ├── fortinet-fortigate-panel.yaml
│   ├── globalprotect-panel.yaml
│   ├── grafana-detect.yaml
│   ├── jenkins-asyncpeople.yaml
│   ├── jmx-console.yaml
│   ├── kubernetes-pods.yaml
│   ├── mongo-express-web-gui.yaml
│   ├── parallels-html-client.yaml
│   ├── phpmyadmin-panel.yaml
│   ├── pulse-secure-panel.yaml
│   ├── rabbitmq-dashboard.yaml
│   ├── sap-netweaver-detect.yaml
│   ├── sap-recon-detect.yaml
│   ├── sophos-fw-version-detect.yaml
│   ├── supervpn-panel.yaml
│   ├── swagger-panel.yaml
│   ├── tikiwiki-cms.yaml
│   ├── weave-scope-dashboard-detect.yaml
│   └── webeditors.yaml
├── payloads
│   └── CVE-2020-6287.xml
├── security-misconfiguration
│   ├── basic-cors-flash.yaml
│   ├── basic-cors.yaml
│   ├── front-page-misconfig.yaml
│   ├── jira-service-desk-signup.yaml
│   ├── jira-unauthenticated-dashboards.yaml
│   ├── jira-unauthenticated-popular-filters.yaml
│   ├── jira-unauthenticated-projects.yaml
│   ├── jira-unauthenticated-user-picker.yaml
│   ├── rabbitmq-default-admin.yaml
│   ├── rack-mini-profiler.yaml
│   ├── springboot-detect.yaml
│   └── wamp-xdebug-detect.yaml
├── subdomain-takeover
│   ├── detect-all-takeovers.yaml
│   └── s3-subtakeover.yaml
├── technologies
│   ├── bigip-config-utility-detect.yaml
│   ├── citrix-vpn-detect.yaml
│   ├── clockwork-php-page.yaml
│   ├── couchdb-detect.yaml
│   ├── github-enterprise-detect.yaml
│   ├── gitlab-detect.yaml
│   ├── graphql.yaml
│   ├── home-assistant.yaml
│   ├── jaspersoft-detect.yaml
│   ├── jira-detect.yaml
│   ├── liferay-portal-detect.yaml
│   ├── linkerd-badrule-detect.yaml
│   ├── linkerd-ssrf-detect.yaml
│   ├── netsweeper-webadmin-detect.yaml
│   ├── ntlm-directories.yaml
│   ├── prometheus-exposed-panel.yaml
│   ├── s3-detect.yaml
│   ├── sap-netweaver-as-java-detect.yaml
│   ├── sap-netweaver-detect.yaml
│   ├── sql-server-reporting.yaml
│   ├── tech-detect.yaml
│   ├── weblogic-detect.yaml
│   └── werkzeug-debugger-detect.yaml
├── tokens
│   ├── amazon-mws-auth-token-value.yaml
│   ├── aws-access-key-value.yaml
│   ├── google-api-key.yaml
│   ├── http-username-password.yaml
│   ├── mailchimp-api-key.yaml
│   └── slack-access-token.yaml
├── vulnerabilities
│   ├── cached-aem-pages.yaml
│   ├── couchdb-adminparty.yaml
│   ├── crlf-injection.yaml
│   ├── discourse-xss.yaml
│   ├── git-config-nginxoffbyslash.yaml
│   ├── ibm-infoprint-directory-traversal.yaml
│   ├── microstrategy-ssrf.yaml
│   ├── moodle-filter-jmol-lfi.yaml
│   ├── moodle-filter-jmol-xss.yaml
│   ├── nginx-module-vts-xss.yaml
│   ├── open-redirect.yaml
│   ├── oracle-ebs-bispgraph-file-access.yaml
│   ├── pdf-signer-ssti-to-rce.yaml
│   ├── rce-shellshock-user-agent.yaml
│   ├── rce-via-java-deserialization.yaml
│   ├── springboot-actuators-jolokia-xxe.yaml
│   ├── symfony-debugmode.yaml
│   ├── tikiwiki-reflected-xss.yaml
│   ├── tomcat-manager-pathnormalization.yaml
│   ├── twig-php-ssti.yaml
│   ├── wordpress-duplicator-path-traversal.yaml
│   ├── wordpress-wordfence-xss.yaml
│   └── x-forwarded-host-injection.yaml
└── workflows
    ├── bigip-pwner-workflow.yaml
    ├── jira-exploitaiton-workflow.yaml
    ├── liferay-rce-workflow.yaml
    ├── netsweeper-preauth-rce-workflow.yaml
    ├── rabbitmq-workflow.yaml
    ├── sap-netweaver-workflow.yaml
    └── springboot-pwner-workflow.yaml
```

</details>

13 directories, **204 templates**. 

Please navigate to https://nuclei.projectdiscovery.io for detailed documentation to build new and your own custom templates and many example templates for easy understanding. 

------
**Notes:** 
1. Use YAMLlint (e.g. [yamllint](http://www.yamllint.com/)) to validate new templates when sending pull requests.
2. Use YAML Formatter (e.g. [jsonformatter](https://jsonformatter.org/yaml-formatter)) to format new templates when sending pull requests.

Thanks again for your contribution and keeping the community vibrant. :heart:
