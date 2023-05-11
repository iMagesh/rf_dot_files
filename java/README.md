# Checkstyle

### Installation

#### Maven

```
<reporting>
    <plugins>
        <plugin>
            <groupId>org.apache.maven.plugins</groupId>
            <artifactId>maven-checkstyle-plugin</artifactId>
            <version>3.0.0</version>
            <configuration>
                <configLocation>checkstyle.xml</configLocation>
            </configuration>
        </plugin>
    </plugins>
</reporting>
```

#### Gradle

```
apply plugin: 'checkstyle'
checkstyle {
    toolVersion 'toolVersion'
    configFile file("config/checkstyle/checkstyle.xml")
}
checkstyleMain {
    source ='src/main/java'
}
checkstyleTest {
    source ='src/test/java'
}
```

This plugin comes with two predefined checks, a Sun-style check, and a Google-style check. The default check for a project is sun_checks.xml.
