---
layout: default
title: test index
---

# posts
{% for post in site.posts %}
{{ post.date | date_to_string }} [{{ post.title }}]({{ post.url }})
{% endfor %}

# title 1
 something

## title 2
   something else

### title 3
   another something


using markdown file with md extension and line numbers

xml code

{% highlight xml %}
<modelVersion>4.0.0</modelVersion>
      <groupId>fr.usi2011.cassandra</groupId>
      <artifactId>usi2011-jaxio</artifactId>
      <version>0.0.1-SNAPSHOT</version>
      <packaging>jar</packaging>
      <name>usi2011-jaxio</name>
      ...      
{% endhighlight %}

java code

{% highlight java linenos %}
@ImportResource("classpath*:/applicationContext.xml")
@ComponentScan(basePackageClasses = Main.class)
public static class DefaultConfiguration {
    @Bean
    public AnnotationMBeanExporter mbeanExporter() {
        AnnotationMBeanExporter exporterThatCatchesExceptions = new AnnotationMBeanExporter();
        exporterThatCatchesExceptions.setRegistrationBehavior(REGISTRATION_IGNORE_EXISTING);
        exporterThatCatchesExceptions.setEnsureUniqueRuntimeObjectNames(false);
        return exporterThatCatchesExceptions;
    }
}
{% endhighlight %}

end

