# Antonio Trento 

Blog sul web maketing e business su web

## Blog post template

Per ogni post del blog sono configurabili e personalizzabili inserendo l'apposito campo nel template del post: 

* un social locker
* un welcome mat
* hellobar
* popup exitintent
* calltoaction
* socialtagline

```

---
layout: post
category : nome categoria (cartella contenuta in _posts)
tagline: "I migliori hosting per wordpress e jekyll nel 2018"
tags : [hosting, web sites, web business]
locker: <p>Codice html da visualizzare nel locker.</p>
img : indirizzo dell'immagine contenuta in ../assets/images
author : Antonio Trento
css: 
js:  
keywords: hosting, websites, business, web
canonical: https://lantoniotrento.github.io/hosting/2017/10/13/i-migliori-provider-hosting-del-2018
calltoaction: <span>html per testo call to action a fine articolo del blog</span>
socialtagline: testo contenuto prima dei bottoni social share 
exitintent: <a href="#">html per attivare popup exitintent (meglio usare un immagine altrimenti bisogna modificare css)</a>
hellobar: yes
welcomemat:   <div>html del welcom mat</div>

---
{% include JB/setup %}

<!--more-->

# Titolo

contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto 

{% include social-locker.html %} //posizionamento social locker nella pagina

 contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto contenuto

{% social-share.html %} //posizionamento social share nella pagina

```

