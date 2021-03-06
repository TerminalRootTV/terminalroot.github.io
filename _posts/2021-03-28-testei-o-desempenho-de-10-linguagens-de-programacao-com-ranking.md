---
layout: post
title: "Testei o Desempenho de 10 Linguagens de Programação com Ranking"
date: 2021-03-28 23:46:20
image: '/assets/img/programacao/langs.jpg'
description: 'E a mais veloz foi ...'
icon: 'ion:terminal-sharp'
iconname: 'programação'
tags:
- cpp
- linguagemc
- python
- java
- php
- ruby
- go
- javascript
- rust
- shellscript
---

![Testei o Desempenho de 10 Linguagens de Programação com Ranking](/assets/img/programacao/langs.jpg)

🔊 Nesse vídeo testamos a velocidade das linguagens de programação:

+ [Python](https://terminalroot.com.br/tags#python)
+ [JavaScript](https://terminalroot.com.br/tags#javascript)
+ [Rust](https://terminalroot.com.br/tags#rust)
+ [Shell Script](https://terminalroot.com.br/shell)
+ [Java](https://terminalroot.com.br/tags#java)
+ [C++](https://terminalroot.com.br/cpp) 
+ [C](https://terminalroot.com.br/tags#linguagemc)
+ [PHP](https://terminalroot.com.br/php)
+ [Ruby](https://terminalroot.com.br/tags#ruby)
+ [Go](https://terminalroot.com.br/tags#go)

E ao final criamos um ranking com Awk .

# Assista ao Vídeo
<iframe width="910" height="390" src="https://www.youtube.com/embed/spLIBqiv2Og" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<!-- QUADRADO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:inline-block;width:336px;height:280px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

---

# Código das Linguagens

### 01. SHELL SCRIPT `vim sh.sh`
{% highlight bash %}
for i in {1..1000000};
  do
    echo -en "${i}Ok\r"
done
{% endhighlight %}
+ Rodar: `sh sh.sh`
+ Testar: `time sh sh.sh`


---

### 02. PHP `vim php.php`
{% highlight php %}
<?php

for( $i = 0; $i <= 1000000; $i++ ){
  echo "{$i}Ok\r";
}
{% endhighlight %}
+ Rodar: `php php.php`
+ Testar: `time php php.php`

---

### 03. JAVASCRIPT `vim js.js`
{% highlight js %}
for( var i = 0; i <= 1000000; i++ ){
  process.stdout.write( i + "Ok\r");
}
{% endhighlight %}
+ Rodar: `node js.js`
+ Testar: `time node js.js`

<!-- MINI ANÚNCIO -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<!-- Games Root -->
<ins class="adsbygoogle"
style="display:inline-block;width:730px;height:95px"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="5351066970"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

---

### 04. RUBY `vim ruby.rb`
{% highlight ruby %}
for i in 1..1000000 do
 print "#{i}Ok\r"
end
{% endhighlight %}
+ Rodar: `ruby ruby.rb`
+ Testar: `time ruby ruby.rb`

---

### 05. PYTHON `vim python.py`
{% highlight python %}
for i in range(1000001):
    print( str(i) + "Ok\r", end='' )
{% endhighlight %}
+ Rodar: `python python.py`
+ Testar: `time python python.py`

---

### 06. JAVA `vim java.java`
{% highlight java %}
class java {
  public static void main ( String args[] ) {
    for ( int i = 0; i <= 1000000 ; i++ ){
      System.out.print( i + "Ok\r" );
    }  
  }
}
{% endhighlight %}
+ Rodar: `javac java.java && java java`
+ Testar: `time java java`

---

<!-- RETANGULO LARGO 2 -->
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
style="display:block; text-align:center;"
data-ad-layout="in-article"
data-ad-format="fluid"
data-ad-client="ca-pub-2838251107855362"
data-ad-slot="8549252987"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>

### 07. GO `vim go.go`
{% highlight go %}
package main
import (
  "fmt"
)

func main() {
  for i := 0; i <= 1000000; i++{
    fmt.Printf("%vOK\r", i)
  }
  
}
{% endhighlight %}
+ Rodar: `go build go.go && ./go`
+ Testar: `time ./go`

---

### 08. C++ `vim cpp.cpp`
{% highlight cpp %}
#include <iostream>

int main(){
  for (int i = 0; i <= 1000000; i++) {
   std::cout << i << "Ok\r"; 
  }
  return 0;
}
{% endhighlight %}
+ Rodar: `g++ cpp.cpp && ./a.out`
+ Testar: `time ./a.out`

---

### 09. RUST `vim rust.rs`
{% highlight rust %}
fn main() {
 for i in 0..1000001 {
    print!("{}Ok\r", i);
 }
}
{% endhighlight %}
+ Rodar: `rustc rust.rs && ./rust`
+ Testar: `time ./rust`

---

### 10. C `vim c.c`
{% highlight c %}
i#include <stdio.h>

int main(){
  for (int i = 0; i <= 1000000; i++) {
    printf("%iOk\r", i);
  }
  return 0;
}
{% endhighlight %}
+ Rodar: `gcc c.c && ./a.out`
+ Testar: `time ./a.out`

# Paz!

