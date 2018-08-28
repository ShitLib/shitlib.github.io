---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
---

## ShitLib (Oh Shit!)

### The only library you hope to remove!
The library that helps you remember about things done bad.
With ShitLib you will be always aware of the shitty code inside your application.

### Installation
Import the library, proabably the smallest library you'll every see
Maven
{% highlight xml %}
<dependency>
    <groupId>io.github.shitlib</groupId>
    <artifactId>shitlib-java</artifactId>
    <version>1</version>
</dependency>
{% endhighlight %}
Gradle
```groovy
dependencies {
    implementation 'io.github.shitlib:shitlib-java:1'
}
```

### Usage
Are you writing unwanted code, antipatterns, magic numbers?
Are you scared about what you are doing?
Use ShitLib to refer your shitty code so you will remember it.
How? Remove ShitLib and your code will not compile anymore until you will remove all of the shitty code.


Oh your boss forced you to get the first element of a list and you know that it's wrong: You can use OhShit!

```java
import static io.github.shitlib.java.OhShit.*;

class MyBeautifulClass {
    
    List<String> elements;//with some elements inside
    
    void iDontWantDoThisButWeMustReleaseASAP() {
        String element = elements.get(_0);//<--- OhShit Constant
        doSomeThing(element);
    }
    
    void doSomeThing(String element) {
        //everything
    }
}
```  

Maybe are you thinking where is the convenience in using this lib.
It's simple, this is the most useful library when it is deleted.
After that your project will not compile and you will be immediately aware of what to do.
Fix it!

Other way to use ShitLib? Let's give a try to the method API

```java
import static io.github.shitlib.java.OhShit.*;

class MyBeautifulUnConfigurableClass {
    
    public static final int MAX_PASSWORD_SIZE = ohShit(7);//I cannot parameterize now
    
    public void setPassword(String password) {
         if (password.length() > MAX_PASSWORD_SIZE) {
              throw new InvalidArgumentException("password");
         }
    }
}
```  

### News
  * 20-02-2018 First release on maven central repo

### Vote for the next step
  * [Add new methods](https://strawpoll.com/p55b3gp8): ``crap``, ``holyCow``, ``wtf``, ``omg``;
  * [Add new classes](https://strawpoll.com/kfbsxpkw): ``Crap``, ``HolyCow``, ``WTF``, ``OMG``.
