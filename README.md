# VMS Maven Archetype

Maven template that creates a minimal project as a starting point for new application service.

## Usage

To generate a project, adjust the following command line to your needs:

- Adjust `appName=engine` to define the application name.
- Lookup the list of [available properties](#available-properties) to see if there's more you want to adjust.

```shell
mvn -B org.apache.maven.plugins:maven-archetype-plugin:3.2.1:generate \
 -D archetypeGroupId=olegood.vms \
 -D archetypeArtifactId=vms-maven-archetype \
 -D archetypeVersion=1.0 \
 -D appName=engine
```

## Available Properties

| Name            | Default                  | Description                                                                                                                    |
|-----------------|--------------------------|--------------------------------------------------------------------------------------------------------------------------------|
| `appName`       |                          | Application name (e.g. `engine`).                                                                                              |
| `artifactId`    | `vms-${appName}`         | Base Maven artifact ID (e.g. `vms-engine`).                                                                                    |
| `groupId`       | `olegood.vms.${appName}` | Base Maven group ID (e.g. `olegood.vms.engine`).                                                                               |
| `javaVersion`   | `17`                     | Java Development Kit version.                                                                                                  |
| `package`       | `${groupId}`             | Java Source Package (e.g. `olegood.vms.engine`).                                                                               |
| `parentVersion` | `2.7.3`                  | Spring Boot Starter Parent ([latest](https://mvnrepository.com/artifact/org.springframework.boot/spring-boot-starter-parent)). |
| `version`       | `1.0-SNAPSHOT`           | Project version (e.g. `1.0-SNAPSHOT`).                                                                                         |

**Note:** sorted alphabetically.

## License

The code in this repository is all under either the MIT license, or a license compatible with the MIT license.
See the [LICENSE](LICENSE) file for more information.

## Code of Conduct

Please refer to [Code of Conduct](CODE_OF_CONDUCT.md).

## Additional Resources

- [Apache Maven](https://maven.apache.org/)
- [Maven Archetype](https://maven.apache.org/archetype/index.html)
- [Maven Archetype Plugin](https://maven.apache.org/archetype/maven-archetype-plugin/usage.html)
- [Spring Boot Starter Parent](https://docs.spring.io/spring-boot/docs/current/reference/html/getting-started.html)