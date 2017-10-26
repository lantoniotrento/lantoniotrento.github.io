# Antonio Trento 

Blog sul web maketing e business su web

Sul file _config.yaml si può configurare il sistema che comprende

* Google AD Sense
* Google Analytics
* Google tag manager
* Google Optimize
* Area contatti e social
* https://zotabox.com/ (per integrarlo devi modificare il link nel codice zotabox js delle pagine ../_includes/bootstrap/default.html - default-index-html - default-page.html - default-signup.html)

Sono presenti 3 tipologie di layout per le  pagine web

* post (carica [shrift](http://snip.ly/sp2i7))
* index (carica [template areal](http://snip.ly/dtv6t))
* page (carica [bootstrap 4](http://snip.ly/f5kn9))
* signup (carica template [eventually](http://snip.ly/2a0sm))

## Blog post template

Per ogni post del blog sono configurabili e personalizzabili inserendo l'apposito campo nel template del post: 

* un social locker
* un welcome mat
* hellobar
* popup exitintent
* calltoaction
* socialtagline
* css esterno (cartella upload /assets/css)
* js esterno (cartella upload /assets/js)
../_posts/categoria/YYYY-MM-DD-nome-eccezionale-post.md


```

---
layout: post
category : nome categoria (cartella contenuta in _posts)
tagline: "I migliori hosting per wordpress e jekyll nel 2018"
tags : [hosting, web sites, web business]
locker: <p>Codice html da visualizzare nel locker.</p>
img : indirizzo dell'immagine contenuta in ../assets/images
author : Antonio Trento
css: indirizzo dell'immagine contenuta in ../assets/css)
js:  indirizzo dell'immagine contenuta in ../assets/js)
keywords: hosting, websites, business, web
canonical: https://lantoniotrento.github.io/hosting/2017/10/13/i-migliori-provider-hosting-del-2018
calltoaction: <span>html per testo call to action a fine articolo del blog</span>
socialtagline: testo contenuto prima dei bottoni social share 
exitintent: <a href="#">html per attivare popup exitintent (meglio usare un immagine altrimenti bisogna modificare css)</a>
hellobar: yes (hello bar on/off)
welcomemat:   <div>html del welcom mat</div>
wm-image-1: https://lantoniotrento.github.io/assets/images/cover-bg-1.jpg //indirizzi assoluti immagini di sfondo
wm-image-2: https://lantoniotrento.github.io/assets/images/cover-bg-1.jpg
wm-image-3: https://lantoniotrento.github.io/assets/images/cover-bg-1.jpg


---
{% include JB/setup %}

<!--more-->

# Titolo

contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto 

contenuto contenuto contenuto contenuto

{% include social-locker.html %} //posizionamento social locker nella pagina

 contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto 
 contenuto contenuto contenuto contenuto 

{% include social-share.html %} //posizionamento social share nella pagina

{% include sign-up.html %} //posizionamento di un banner di iscrizione lista

```

Per le pagine sono stati prvisti tre layout diversi:

* ### Layout index carica stili CSS della pagina https://lantoniotrento.github.io
```
---
layout: index
title: Antonio Trento
tagline: User experience, web marketing, web design
css: 
js:
keywords: Graphic design, web marketing, web design, user experience
canonical: https://antoniotrento.github.io
---
{% include JB/setup %}
```

* ### Layout page carica stili CSS della pagina https://lantoniotrento.github.io/blog
```
---
layout: page
title: Pagina di test
tagline: commento test
css: 
js:
keywords: Graphic design, web marketing, web design, user experience
canonical: 
---
{% include JB/setup %}
```

* ### Layout signup carica stili CSS della pagina https://lantoniotrento.github.io/signup
```
---
layout: signup
title: Signup
tagline: 
css: 
js: eventually/main.js
keywords: business, web marketing, money
canonical:
---
{% include JB/setup %}
```

### Tracciamento link

```
<a href="http://www.example.com" onclick="trackOutboundLink('http://www.example.com'); return false;">Non perderti example.com</a>
```
### Post scheduler

Il  sito web è munito di post scheduler grazie alle funzionalità di [](https://serverless.com) e [Amazon AWS](https://aws.amazon.com/it/) utilizzando le  funzionalità di [post scheduler](https://serverless.com/blog/static-site-post-scheduler/) per  sfruttarlo anche tu segui le guide vidio di serverless

> Per creare un nuovo post in schedule, va crato un novo brach del progetto, creare un nuovo post nella cartella /_posts/categoria/ salvare il post ed i dati correlati ed effetturare il merge del branch sul brach master. Poi da  master andando su pull request commentare la richiesta di merge con schedule(MM/DD/YYYY H:MM pm), serverless effettuerà lo schedule all'ora desiderata
