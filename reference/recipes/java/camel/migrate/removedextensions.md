# Remove non existing camel-quarkus extensions

**org.openrewrite.java.camel.migrate.removedExtensions**

_Removal of maven dependencies for extension, which are no longer part of Camel 3.x._

## Recipe source

[GitHub](https://github.com/search?type=code&q=org.openrewrite.java.camel.migrate.removedExtensions), [Issue Tracker](https://github.com/openrewrite/rewrite-third-party/issues), [Maven Central](https://central.sonatype.com/artifact/org.openrewrite.recipe/rewrite-third-party/0.7.0/jar)

* groupId: org.openrewrite.recipe
* artifactId: rewrite-third-party
* version: 0.7.0

{% hint style="info" %}
This recipe is composed of more than one recipe. If you want to customize the set of recipes this is composed of, you can find and copy the GitHub source for the recipe from the link above.
{% endhint %}

## Definition

{% tabs %}
{% tab title="Recipe List" %}
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-activemq`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-activemq`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-atmos`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-avro-rpc`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-caffeine-lrucache`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-datasonnet`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-dozer`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-elasticsearch-rest`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-gora`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-hbase`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-iota`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-jbpm`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-jclouds`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-johnzon`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-microprofile-metrics`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-milo`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-opentracing`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-optaplanner`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-rabbitmq`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-smallrye-reactive-messaging`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-solr`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-tika`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-vm`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-xmlsecurity`
* [Remove Maven dependency](../../../maven/removedependency.md)
  * groupId: `org.apache.camel.quarkus`
  * artifactId: `camel-quarkus-xstream`

{% endtab %}

{% tab title="Yaml Recipe List" %}
```yaml
---
type: specs.openrewrite.org/v1beta/recipe
name: org.openrewrite.java.camel.migrate.removedExtensions
displayName: Remove non existing camel-quarkus extensions
description: Removal of maven dependencies for extension, which are no longer part of Camel 3.x.
recipeList:
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-activemq
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-activemq
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-atmos
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-avro-rpc
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-caffeine-lrucache
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-datasonnet
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-dozer
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-elasticsearch-rest
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-gora
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-hbase
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-iota
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-jbpm
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-jclouds
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-johnzon
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-microprofile-metrics
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-milo
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-opentracing
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-optaplanner
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-rabbitmq
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-smallrye-reactive-messaging
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-solr
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-tika
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-vm
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-xmlsecurity
  - org.openrewrite.maven.RemoveDependency:
      groupId: org.apache.camel.quarkus
      artifactId: camel-quarkus-xstream

```
{% endtab %}
{% endtabs %}

## Usage

This recipe has no required configuration options. It can be activated by adding a dependency on `org.openrewrite.recipe:rewrite-third-party:0.7.0` in your build file or by running a shell command (in which case no build changes are needed): 
{% tabs %}
{% tab title="Gradle" %}
1. Add the following to your `build.gradle` file:
{% code title="build.gradle" %}
```groovy
plugins {
    id("org.openrewrite.rewrite") version("6.21.1")
}

rewrite {
    activeRecipe("org.openrewrite.java.camel.migrate.removedExtensions")
    exportDatatables = true
}

repositories {
    mavenCentral()
}

dependencies {
    rewrite("org.openrewrite.recipe:rewrite-third-party:0.7.0")
}
```
{% endcode %}
2. Run `gradle rewriteRun` to run the recipe.
{% endtab %}

{% tab title="Gradle init script" %}
1. Create a file named `init.gradle` in the root of your project.
{% code title="init.gradle" %}
```groovy
initscript {
    repositories {
        maven { url "https://plugins.gradle.org/m2" }
    }
    dependencies { classpath("org.openrewrite:plugin:6.21.1") }
}
rootProject {
    plugins.apply(org.openrewrite.gradle.RewritePlugin)
    dependencies {
        rewrite("org.openrewrite.recipe:rewrite-third-party:0.7.0")
    }
    rewrite {
        activeRecipe("org.openrewrite.java.camel.migrate.removedExtensions")
        exportDatatables = true
    }
    afterEvaluate {
        if (repositories.isEmpty()) {
            repositories {
                mavenCentral()
            }
        }
    }
}
```
{% endcode %}
2. Run the recipe.
{% code title="shell" overflow="wrap"%}
```shell
gradle --init-script init.gradle rewriteRun
```
{% endcode %}
{% endtab %}
{% tab title="Maven POM" %}
1. Add the following to your `pom.xml` file:
{% code title="pom.xml" %}
```xml
<project>
  <build>
    <plugins>
      <plugin>
        <groupId>org.openrewrite.maven</groupId>
        <artifactId>rewrite-maven-plugin</artifactId>
        <version>5.39.2</version>
        <configuration>
          <exportDatatables>true</exportDatatables>
          <activeRecipes>
            <recipe>org.openrewrite.java.camel.migrate.removedExtensions</recipe>
          </activeRecipes>
        </configuration>
        <dependencies>
          <dependency>
            <groupId>org.openrewrite.recipe</groupId>
            <artifactId>rewrite-third-party</artifactId>
            <version>0.7.0</version>
          </dependency>
        </dependencies>
      </plugin>
    </plugins>
  </build>
</project>
```
{% endcode %}
2. Run `mvn rewrite:run` to run the recipe.
{% endtab %}

{% tab title="Maven Command Line" %}

You will need to have [Maven](https://maven.apache.org/download.cgi) installed on your machine before you can run the following command.

{% code title="shell" overflow="wrap" %}
```shell
mvn -U org.openrewrite.maven:rewrite-maven-plugin:run -Drewrite.recipeArtifactCoordinates=org.openrewrite.recipe:rewrite-third-party:RELEASE -Drewrite.activeRecipes=org.openrewrite.java.camel.migrate.removedExtensions -Drewrite.exportDatatables=true
```
{% endcode %}
{% endtab %}
{% tab title="Moderne CLI" %}
You will need to have configured the [Moderne CLI](https://docs.moderne.io/moderne-cli/cli-intro) on your machine before you can run the following command.

{% code title="shell" %}
```shell
mod run . --recipe removedExtensions
```
{% endcode %}
{% endtab %}
{% endtabs %}

## See how this recipe works across multiple open-source repositories

[![Moderne Link Image](/.gitbook/assets/ModerneRecipeButton.png)](https://app.moderne.io/recipes/org.openrewrite.java.camel.migrate.removedExtensions)

The community edition of the Moderne platform enables you to easily run recipes across thousands of open-source repositories.

Please [contact Moderne](https://moderne.io/product) for more information about safely running the recipes on your own codebase in a private SaaS.
## Data Tables

### Source files that had results
**org.openrewrite.table.SourcesFileResults**

_Source files that were modified by the recipe run._

| Column Name | Description |
| ----------- | ----------- |
| Source path before the run | The source path of the file before the run. `null` when a source file was created during the run. |
| Source path after the run | A recipe may modify the source path. This is the path after the run. `null` when a source file was deleted during the run. |
| Parent of the recipe that made changes | In a hierarchical recipe, the parent of the recipe that made a change. Empty if this is the root of a hierarchy or if the recipe is not hierarchical at all. |
| Recipe that made changes | The specific recipe that made a change. |
| Estimated time saving | An estimated effort that a developer to fix manually instead of using this recipe, in unit of seconds. |
| Cycle | The recipe cycle in which the change was made. |

### Source files that errored on a recipe
**org.openrewrite.table.SourcesFileErrors**

_The details of all errors produced by a recipe run._

| Column Name | Description |
| ----------- | ----------- |
| Source path | The file that failed to parse. |
| Recipe that made changes | The specific recipe that made a change. |
| Stack trace | The stack trace of the failure. |

### Recipe performance
**org.openrewrite.table.RecipeRunStats**

_Statistics used in analyzing the performance of recipes._

| Column Name | Description |
| ----------- | ----------- |
| The recipe | The recipe whose stats are being measured both individually and cumulatively. |
| Source file count | The number of source files the recipe ran over. |
| Source file changed count | The number of source files which were changed in the recipe run. Includes files created, deleted, and edited. |
| Cumulative scanning time | The total time spent across the scanning phase of this recipe. |
| 99th percentile scanning time | 99 out of 100 scans completed in this amount of time. |
| Max scanning time | The max time scanning any one source file. |
| Cumulative edit time | The total time spent across the editing phase of this recipe. |
| 99th percentile edit time | 99 out of 100 edits completed in this amount of time. |
| Max edit time | The max time editing any one source file. |

