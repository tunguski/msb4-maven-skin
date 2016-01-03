#### [Bootstrap themes from Bootswatch][themes]

[![Bootswatch themes](images/carousel-themes.png)][themes]

Select a free theme for your website from an excellent gallery at [Bootswatch][bootswatch].
Out of the box support for these and other custom [Bootstrap][bootstrap] themes.


#### [Page layouts][msb4-layouts]

[![Page layouts](images/carousel-layouts.jpg)][msb4-layouts]

Write plain text in Markdown or APT, then set different layouts to your page sections.


#### [Modern skin][msb4-misc]

[![Modern skin](images/carousel-components.jpg)][msb4-misc]

Msb4 skin uses modern components from Bootstrap and other libraries, upgrades Maven generated
site and provides further enhancements.


#### [New Velocity tools][msb4-tools]

[![Msb4 Velocity tools](images/carousel-tools.png)][msb4-tools]

The skin adds a library of new Velocity tools to use in your own Maven template: rewrite HTML code,
support per-page configurations and more!


[bootswatch]: http://bootswatch.com
[bootstrap]: http://getbootstrap.com
[themes]: skin/themes/
[msb4-layouts]: skin/layouts.html
[msb4-misc]: skin/misc.html
[msb4-tools]: msb4-velocity-tools/


---


## Get it now

To use Msb4 skin in your Maven site, [add it to site.xml][msb4-usage]:

```xml
<skin>
  <groupId>pl.matsuo.maven.skins</groupId>
  <artifactId>msb4-maven-skin</artifactId>
  <version>0.1.0-SNAPSHOT</version>
</skin>
```

Furthermore, the skin requires accompanying [Msb4 Velocity tools][msb4-tools] as a dependency
as well as Apache Velocity 1.7.
[Add them as dependencies][msb4-usage] to `maven-site-plugin`.

[Full usage instructions &raquo;][msb4-usage]

[msb4-usage]: skin/


## Responsive layouts

Write your pages in [APT or Markdown][doxia-formats], then restructure them using Msb4 skin
[layouts][msb4-layouts]:

-   **Carousel** - spinning image slideshow
-   **Thumbnails** - showcase your image gallery
-   **Columns** - multi-column text
-   **Sidebar** - wrap into a sidebar
-   **Body** - text as it has been written

Partition the page into sections using `<hr/>` elements, and define preferred layouts for each section in `site.xml`. Msb4 skin is responsive thanks to [Bootstrap][bootstrap], so the layouts
will be rearranged automatically for readability on small screens.

[Read more about layouts in the documentation &raquo;][msb4-layouts]

[doxia-formats]: http://maven.apache.org/doxia/references/index.html


## Themes

The skin theme can be [switched easily][themes]: just select a Bootstrap theme
to give an easy makeover for your Maven site.

-   **Default** - use the default [Bootstrap][bootstrap] theme
-   **Bootswatch** - select an excellent free theme from [Bootswatch][bootswatch]
-   **Custom** - create your own Bootstrap theme with [existing tools][bootstrap-custom]

**Need to change something?** Extend the skin with custom `site.css` file in your project, and
[reuse it for multi-module site][msb4-multi].

[How to select a theme &raquo;][themes]

[bootstrap-custom]: http://getbootstrap.com/customize
[msb4-multi]: skin/multi-module.html


## Configure

Msb4 is very configurable: many features and components can be disabled, and optional
enhancements enabled using [configuration in `site.xml`][msb4-config]:

-   **Table of contents** - display ToC for each page: top bar or sidebar
-   **Menus** - filter Maven menus and select what to display in top or bottom navigation
-   **Code highlight** - syntax colouring for code snippets
-   **Image preview** - display images in pop-ups
-   ... [and more][msb4-config]

Check out the [documentation][msb4-config] for all the features. Every configuration option
can be applied on a _per-page_ basis!

[msb4-config]: skin/config.html


---


## Velocity tools

Msb4 skin provides custom Velocity tools library to be used in Maven site template:

-   **`SkinConfigTool`** - convenient access to custom configuration options (global and per-page)
-   **`HtmlTool`** - query and modify HTML text
-   **`URITool`** - use Java URIs in the template

To enable these tools for any skin, add `msb4-velocity-tools` dependency to
`maven-site-plugin` in the POM.

[Read more about usage and browse the Javadoc &raquo;][msb4-tools]


---


### About

Msb4 Maven skin is an [Apache Maven site][mvn-site] skin built on [Bootstrap 4.0][bootstrap].

The code is [open source][msb4-github] and licensed under [Apache license][apache-license].
The skin can be used freely for your Maven projects.

[Contribute][contribute] by reporting issues, suggesting new features, or forking the
Git repository on GitHub and adding some good code!

In the end, if you _really really_ like the skin and want to support the author, I will
be glad to [accept a small donation][donate].

[mvn-site]: http://maven.apache.org/guides/mini/guide-site.html
[apache-license]: http://www.apache.org/licenses/LICENSE-2.0
[contribute]: contribute.html
[msb4-github]: http://github.com/tunguski/msb4-maven-skin/
[donate]: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&amp;hosted_button_id=QWKNRFZH52828
