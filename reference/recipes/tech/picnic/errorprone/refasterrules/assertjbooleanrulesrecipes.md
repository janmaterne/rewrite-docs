# `AssertJBooleanRules` Refaster recipes

**tech.picnic.errorprone.refasterrules.AssertJBooleanRulesRecipes**

_Refaster template recipes for `tech.picnic.errorprone.refasterrules.AssertJBooleanRules`. [Source](https://error-prone.picnic.tech/refasterrules/AssertJBooleanRules)._

## Recipe source

[GitHub](https://github.com/search?type=code&q=tech.picnic.errorprone.refasterrules.AssertJBooleanRulesRecipes), [Issue Tracker](https://github.com/openrewrite/rewrite-third-party/issues), [Maven Central](https://central.sonatype.com/artifact/org.openrewrite.recipe/rewrite-third-party/0.7.0/jar)

* groupId: org.openrewrite.recipe
* artifactId: rewrite-third-party
* version: 0.7.0

{% hint style="info" %}
This recipe is composed of more than one recipe. If you want to customize the set of recipes this is composed of, you can find and copy the GitHub source for the recipe from the link above.
{% endhint %}

## Definition

{% tabs %}
{% tab title="Recipe List" %}
* [Refaster template `AssertJBooleanRules.AbstractBooleanAssertIsEqualTo`](../../../../tech/picnic/errorprone/refasterrules/assertjbooleanrulesrecipes$abstractbooleanassertisequaltorecipe.md)
* [Refaster template `AssertJBooleanRules.AbstractBooleanAssertIsNotEqualTo`](../../../../tech/picnic/errorprone/refasterrules/assertjbooleanrulesrecipes$abstractbooleanassertisnotequaltorecipe.md)
* [Refaster template `AssertJBooleanRules.AbstractBooleanAssertIsTrue`](../../../../tech/picnic/errorprone/refasterrules/assertjbooleanrulesrecipes$abstractbooleanassertistruerecipe.md)
* [Refaster template `AssertJBooleanRules.AssertThatBooleanIsTrue`](../../../../tech/picnic/errorprone/refasterrules/assertjbooleanrulesrecipes$assertthatbooleanistruerecipe.md)
* [Refaster template `AssertJBooleanRules.AbstractBooleanAssertIsFalse`](../../../../tech/picnic/errorprone/refasterrules/assertjbooleanrulesrecipes$abstractbooleanassertisfalserecipe.md)
* [Refaster template `AssertJBooleanRules.AssertThatBooleanIsFalse`](../../../../tech/picnic/errorprone/refasterrules/assertjbooleanrulesrecipes$assertthatbooleanisfalserecipe.md)

{% endtab %}

{% tab title="Yaml Recipe List" %}
```yaml
---
type: specs.openrewrite.org/v1beta/recipe
name: tech.picnic.errorprone.refasterrules.AssertJBooleanRulesRecipes
displayName: `AssertJBooleanRules` Refaster recipes
description: Refaster template recipes for `tech.picnic.errorprone.refasterrules.AssertJBooleanRules`. [Source](https://error-prone.picnic.tech/refasterrules/AssertJBooleanRules).
recipeList:
  - tech.picnic.errorprone.refasterrules.AssertJBooleanRulesRecipes$AbstractBooleanAssertIsEqualToRecipe
  - tech.picnic.errorprone.refasterrules.AssertJBooleanRulesRecipes$AbstractBooleanAssertIsNotEqualToRecipe
  - tech.picnic.errorprone.refasterrules.AssertJBooleanRulesRecipes$AbstractBooleanAssertIsTrueRecipe
  - tech.picnic.errorprone.refasterrules.AssertJBooleanRulesRecipes$AssertThatBooleanIsTrueRecipe
  - tech.picnic.errorprone.refasterrules.AssertJBooleanRulesRecipes$AbstractBooleanAssertIsFalseRecipe
  - tech.picnic.errorprone.refasterrules.AssertJBooleanRulesRecipes$AssertThatBooleanIsFalseRecipe

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
    activeRecipe("tech.picnic.errorprone.refasterrules.AssertJBooleanRulesRecipes")
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
        activeRecipe("tech.picnic.errorprone.refasterrules.AssertJBooleanRulesRecipes")
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
            <recipe>tech.picnic.errorprone.refasterrules.AssertJBooleanRulesRecipes</recipe>
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
mvn -U org.openrewrite.maven:rewrite-maven-plugin:run -Drewrite.recipeArtifactCoordinates=org.openrewrite.recipe:rewrite-third-party:RELEASE -Drewrite.activeRecipes=tech.picnic.errorprone.refasterrules.AssertJBooleanRulesRecipes -Drewrite.exportDatatables=true
```
{% endcode %}
{% endtab %}
{% tab title="Moderne CLI" %}
You will need to have configured the [Moderne CLI](https://docs.moderne.io/moderne-cli/cli-intro) on your machine before you can run the following command.

{% code title="shell" %}
```shell
mod run . --recipe AssertJBooleanRulesRecipes
```
{% endcode %}
{% endtab %}
{% endtabs %}

## See how this recipe works across multiple open-source repositories

[![Moderne Link Image](/.gitbook/assets/ModerneRecipeButton.png)](https://app.moderne.io/recipes/tech.picnic.errorprone.refasterrules.AssertJBooleanRulesRecipes)

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

