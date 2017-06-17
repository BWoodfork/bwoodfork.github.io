---
layout: post
title: Clojure for beginners Installing Clojure
categories:
- blog
published: true
---

These are notes for the 'Clojure for beginners - Installing Clojure' screencast.

### Requirements for this installation tutorial:
* A computer running OSX
* Very minimal knowledge of how the commandline works

### What this episode will cover:
 * Installing Java - (Required to run Clojure)
 * Installing Leiningen - A commandline tool used to build and manage Clojure projects.

### Installing Java

In a new terminal window, make sure Java is installed by running:

{% highlight clojure %}
java -version
{% endhighlight %}

Upon running the `java -version` command in your terminal window, you should be presented with something similar
to this message:

{% highlight clojure %}
java version "1.8.0_112"
Java(TM) SE Runtime Environment (build 1.8.0_112-b16)
Java HotSpot(TM) 64-Bit Server VM (build 25.112-b16, mixed mode)

  (comment
   ; This shows my machine's running Java 1.8. If you're running 1.7,
   ; that works too! If you're running anything older
   ; than 1.7, you may want to upgrade your version of Java.
  )
{% endhighlight %}

If you don't have java installed, OSX will prompt you to install it.

Download Java to install it: [Download Java](https://www.java.com/en/download/)

After Java is installed open your terminal window and run `java -version` again. Now,
you should see your version of java output to your console.

### Installing Leiningen

Leiningen is a commandline tool used to build and manage Clojure projects.

In a terminal window, copy and paste the following lines. This will download and install leiningen. It will take a few minutes
to complete. You can copy and paste each line once at a time in order or copy and paste all of the lines into your terminal window.
{% highlight clojure %}
curl https://raw.githubusercontent.com/technomancy/leiningen/stable/bin/lein > lein
sudo mkdir -p /usr/local/bin/
sudo mv lein /usr/local/bin/lein
sudo chmod a+x /usr/local/bin/lein
{% endhighlight %}

After leiningen has installed, let's check to see if it installed properly by using the following command in our terminal window:

{% highlight clojure %}
which lein
{% endhighlight %}

You should see output similar to the following:
{% highlight clojure %}
/usr/local/bin/lein
{% endhighlight %}

This simply gives you the directory that leiningen installed in.

After that, you're all set! You now have Clojure & Leiningen installed on your machine. If you're experiencing download/install issues
with Leingein, please leave a comment under the instructional screencast video for this tutorial and I will do my best to help you figure out
what the problem is. Thanks!
