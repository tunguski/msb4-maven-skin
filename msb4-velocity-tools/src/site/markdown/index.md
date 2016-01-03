# Msb4 Velocity tools

Msb4 skin provides custom tools for [Apache Velocity][velocity] to be used in Maven site
template. These objects are contributed to Velocity context and can be used within the template.
Refer to [Javadoc][javadoc-all] for each tool for more information.

-   **[`SkinConfigTool`][javadoc-config]** (key **$config**)

    Provides a uniform access to Maven site custom configuration options. Supports global and
    per-page configuration. See info on [_per-page configuration_][per-page-info] in Msb4 skin
    for an example of features it brings.
-   **[`HtmlTool`][javadoc-html]** (key **$htmlTool**)

    Provides methods to modify and query HTML text using [jsoup][jsoup] library.
-   **[`URITool`][javadoc-uri]** (key **$uriTool**)

    Provides URI utilities that expose URIs to the template.

[velocity]: http://velocity.apache.org/
[per-page-info]: ../skin/config.html#Per-page_configuration
[jsoup]: http://jsoup.org/

[javadoc-all]: apidocs/
[javadoc-config]: apidocs/pl/matsuo/maven/skins/msb4/SkinConfigTool.html
[javadoc-html]: apidocs/pl/matsuo/maven/skins/msb4/HtmlTool.html
[javadoc-uri]: apidocs/pl/matsuo/maven/skins/msb4/URITool.html


## Usage

To enable these tools, add `msb4-velocity-tools` dependency to `maven-site-plugin` in the POM
file:

```xml
<build>
  <plugins>
    ...
    <plugin>
      <groupId>org.apache.maven.plugins</groupId>
      <artifactId>maven-site-plugin</artifactId>
      <version>4.0</version>
      <dependencies>
        ...
        <dependency>
          <groupId>pl.matsuo.maven.skins</groupId>
          <artifactId>msb4-velocity-tools</artifactId>
          <version>0.1.0-SNAPSHOT</version>
        </dependency>
        ...
      </dependencies>
      ...
    </plugin>
    ...
  </plugins>
</build>
```
