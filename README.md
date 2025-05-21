creedengo-java
===========

_creedengo_ is a collective project aiming to reduce environmental footprint of software at the code level. The goal of
the project is to provide a list of static code analyzers to highlight code structures that may have a negative
ecological impact: energy and resources over-consumption, "fatware", shortening terminals' lifespan, etc.

_creedengo_ is based on evolving catalogs
of https://github.com/green-code-initiative/creedengo-rules-specifications/blob/main/docs/rules[good practices], for various technologies.
This
SonarQube plugin then implements these catalogs as rules for scanning your Java projects.

> ⚠️ This is still a very early stage project. Any feedback or contribution will be highly appreciated. Please
> refer to the contribution section.

https://img.shields.io/badge/License-GPLv3-blue.svg[![License: GPL v3]](https://www.gnu.org/licenses/gpl-3.0)
https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg[![Contributor Covenant]](https://github.com/green-code-initiative/creedengo-common/blob/main/doc/CODE_OF_CONDUCT.md)

🌿 SonarQube Plugins
-------------------

This plugin is part of the creedengo project.\
You can find a list of all our other plugins in
the https://github.com/green-code-initiative/creedengo-rules-specifications#-sonarqube-plugins[creedengo repository]

🚀 Getting Started
------------------

You can give a try with a one command:

```sh
./mvnw verify -Pkeep-running
```

... then you can use Java test project repository to test the environment : see ./src/it/test-projects/creedengo-java-plugin-test-project[Java test project in `./src/it/test-projects/creedengo-java-plugin-test-project`]

NB: To install other `creedengo` plugins, you can :

- add JAVA System properties `Dtest-it.additional-plugins` with a comma separated list of plugin IDs (`groupId:artifactId:version`), or plugins JAR (`file://....`) to install.

  For example :

  ```sh
  ./mvnw verify -Pkeep-running -Dtest-it.additional-plugins=org.sonarsource.javascript:sonar-plugin:10.1.0.21143
  ```
- install different creedengo plugins with Marketplace (inside admin panel of SonarQube)

You can also directly use a https://github.com/green-code-initiative/creedengo-common/blob/main/doc/INSTALL.md#start-sonarqube-if-first-time[all-in-one docker-compose]

... and configure local SonarQube (security config and quality profile : see https://github.com/green-code-initiative/creedengo-common/blob/main/doc/INSTALL.md#configuration-sonarqube[configuration] for more details).

🛒 Distribution
------------------

Ready to use binaries are available https://github.com/green-code-initiative/creedengo-java/releases[from GitHub].

🧩 Compatibility
-----------------

| Plugin version | SonarQube version   | Java version                                                                                   |
|----------------|---------------------|------------------------------------------------------------------------------------------------|
| 1.6.+          | 9.4.+ LTS to 10.6.0 | 11 / 17                                                                                        |
| 1.7.+          | 9.9.+ LTS to 10.6.0 | https://docs.sonarsource.com/sonarqube/9.9/requirements/prerequisites-and-overview/#java[17] |
| 2.+            | 9.9.+ LTS to 25.5.0 | https://docs.sonarsource.com/sonarqube/9.9/requirements/prerequisites-and-overview/#java[17] |

> Compatibility table of versions lower than 1.4.+ are available from the
> main https://github.com/green-code-initiative/creedengo-rules-specifications#-plugins-version-compatibility[creedengo repository].

🤝 Contribution
---------------

check https://github.com/green-code-initiative/creedengo-rules-specifications#-contribution[creedengo repository]

🤓 Main contributors
--------------------

check https://github.com/green-code-initiative/creedengo-rules-specifications#-main-contributors[creedengo repository]

Links
-----

- https://docs.sonarqube.org/latest/analysis/overview/
