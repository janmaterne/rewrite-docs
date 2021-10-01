# Find YAML entries by XPath (deprecated)

** org.openrewrite.yaml.search.FindKeyByXPath**
_Find YAML entries by XPath expression._

## Source

[Github](https://github.com/openrewrite/rewrite), [Issue Tracker](https://github.com/openrewrite/rewrite/issues), [Maven Central](https://search.maven.org/artifact/org.openrewrite/rewrite-yaml/7.14.0/jar)

* groupId: org.openrewrite
* artifactId: rewrite-yaml
* version: 7.14.0

## Options

| Type | Name | Description |
| -- | -- | -- |
| `String` | key | XPath expression used to find matching keys. |


## Usage

This recipe has required configuration parameters. Recipes with required configuration parameters cannot be activated directly. To activate this recipe you must create a new recipe which fills in the required parameters. In your rewrite.yml create a new recipe with a unique name. For example: `com.yourorg.FindKeyByXPathExample`.
Here's how you can define and customize such a recipe within your rewrite.yml:

{% code title="rewrite.yml" %}
```yaml
---
type: specs.openrewrite.org/v1beta/recipe
name: com.yourorg.FindKeyByXPathExample
displayName: Find YAML entries by XPath (deprecated) example
recipeList:
  - org.openrewrite.yaml.search.FindKeyByXPath:
      key: /subjects/kind
```
{% endcode %}


Now that `com.yourorg.FindKeyByXPathExample` has been defined activate it in your build file:

{% tabs %}
{% tab title="Gradle" %}
{% code title="build.gradle" %}
```groovy
plugins {
    id("org.openrewrite.rewrite") version("5.10.0")
}

rewrite {
    activeRecipe("com.yourorg.FindKeyByXPathExample")
}

repositories {
    mavenCentral()
}

```
{% endcode %}
{% endtab %}

{% tab title="Maven" %}
{% code title="pom.xml" %}
```markup
<project>
  <build>
    <plugins>
      <plugin>
        <groupId>org.openrewrite.maven</groupId>
        <artifactId>rewrite-maven-plugin</artifactId>
        <version>4.12.0</version>
        <configuration>
          <activeRecipes>
            <recipe>com.yourorg.FindKeyByXPathExample</recipe>
          </activeRecipes>
        </configuration>
      </plugin>
    </plugins>
  </build>
</project>
```
{% endcode %}
{% endtab %}
{% endtabs %}

Recipes can also be activated directly from the commandline by adding the argument `-DactiveRecipe=com.yourorg.FindKeyByXPathExample`