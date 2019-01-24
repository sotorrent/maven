# releases
Repository for Maven deployment.

[![DOI](https://zenodo.org/badge/134377702.svg)](https://zenodo.org/badge/latestdoi/134377702)

## Usage

If you want to use one of the *SOTorrent* libraries in your project, you first need to configure this GitHub repository as a Maven repository. Simply add the following to your `pom.xml`:

    <repositories>
        <repository>
            <id>sotorrent</id>
            <url>https://raw.github.com/sotorrent/releases/master/</url>
            <snapshots>
                <enabled>true</enabled>
                <updatePolicy>always</updatePolicy>
            </snapshots>
        </repository>
    </repositories>

You can then add, for example, the `string-similarity` library as a dependency:

    <dependencies>
        <dependency>
            <groupId>org.sotorrent</groupId>
            <artifactId>string-similarity</artifactId>
            <version>LATEST</version>
        </dependency>
    </dependencies>
