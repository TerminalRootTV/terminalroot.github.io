---
layout: post
title: 'Desmarcando pacotes do autoremove'
date: '2014-08-03T12:31:00.001-07:00'
image: '/assets/img/linux/new.jpg'
description: 'Algumas vezes quando executamos o comando apt-get autoremove ele lista pacotes ou programas que não queremos que sejam removido'
tags:
- debian
---

![Desmarcando pacotes do autoremove](/assets/img/linux/new.jpg "Desmarcando pacotes do autoremove")

Algumas vezes quando executamos o comando __apt-get autoremove__ ele lista pacotes ou programas que não queremos que sejam removido por gosto ou por motivo de algum erro, logo podemos desmarcar este pacote com o comando __apt-mark__

{% highlight bash %}
apt-mark unmarkauto [pacote]
{% endhighlight %}

Caso o número de pacotes seja grande, vc pode copiar eles do shell, por num editor de texto, organizá-los e criar um loop em Shell Script pra executar o unmark em todos os pacotes, fica de exercício.

Mais informações em

{% highlight bash %}
man apt-mark
{% endhighlight %}

Até a próxima!

<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>

<!-- Informat -->
<ins class="adsbygoogle"
 style="display:block"
 data-ad-client="ca-pub-2838251107855362"
 data-ad-slot="2327980059"
 data-ad-format="auto"
 data-full-width-responsive="true"></ins>

<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>



