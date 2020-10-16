# learning HTML & CSS

##HTML - HyperText Markup Language
Czyli zestaw znacznikiów, które klient (jakaś aplikacja np. przeglądarka) może interpretować i poprawnie wyświetlać

HyperText - bo teksty są interpretowane w ramach protokołu HTTP w przeglądarce  

Markup - bo zawiera znaczniki (tzw. tagi)

Language - może być czytany przez maszynę i człowieka

###Atrybut
```html
<znacznik atrybut="">

np. hiperłącze

<a href="http://google.com" target="_blank"> Link do google </a> target blank otwiera link w nowym oknie

<a href="#sekcja4"> Przejdź do sekcji 4 </a> Przenosi do sekcja4 jeśli <section id="sekcja4">S4</section>

<!-- komentarz -->

<br/> - przenieś do nowej linii

<hr/> - linia pozioma 

<img> src="link do obrazka" alt="tekst alternatywny do obrazka" width="80%" height=""/>
```
jeśli poda się tylko % w szerokośći ro obrazek będzie skalował się razem z przeglądarką (responsywaność) zachowując proporcje (nie podane height)


###Tagi
[więcej tutaj](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

###Elementy blokowe
- zawsze mają znaczniki otwierające i zamykające
- zajmują całą szerokość dokumentu (można to zmienić w css)
```html
<header> górna sekcja strony 

<footer> stopka 

<p> akapity 

<ul> i <ol> listy nieuporządkowna(kropki) i uporządkowana(numerki)

<h1> fo <h6> nagłówki, dobrze żeby h1 był tylko jeden w dokumencie a h2 nie więcej niż 5

<section> sekcje czyli elementy grupujące części strony

<article> merytorycznie odrębne części strony np. artykuły

<aside> elementy treści jeśli nie ma sensu by mogły być wycięte

<nav> najczęściej linki, któe dobrze jest zawrzeć w elemencie <ul> (lista) a każda pozycja listy <li>

<div> element bez znaczenie semantycznego, pełni rolę organizacyjną

<blockquote> większy element który jest cytatem (np. cały paragraf <p>) 
```
###Elementy liniowe
- zajmują przestrzeń wymaganą dla ich treści (można to zmienić w css)

```html
<span> element bez znaczenia semantycznego, do wyróżeninia wizualnego

<a> linki 

<em> ważne treści, pochyla, robot ideksujące rozpoznaje je jako słowa kluczowe

<i> pochylone 

<b> bold

<q> cytat zamyka treść w cudzysłowach

<strong> pogrubienie wizualne
```
#CSS - Cascading Style Sheets
Składnia odpowiadająca za to jak treść HTML się prezentuje - np. kolory fontów, czcionki, rozmieszczenie itd.

##Reguła CSS
kto { co: jak;}  np. 
```html
h1 { color: red;}

#stopka {
    font-family: 'Helvetica', 'Arial';
    margin: 10px 15px;
    color: #009988;
}
```
kto (selektor) - adres htmla do ostylowania np. akapity
co (właściwość) - co chcemy przypisać kolor, wielkość itd
jak (wartość) - wartość np. nazwa koloru

##Osadzanie
###Osadzanie InLine
```html
<p style="font-size: 50px; color : red"> Przykład </p>
```
###Osadzanie w sekcji head
```html
<!doctype html>
<html>
<head>
    <meta charset="utf-8">
    <meta name="description" content="Tutaj jest opis!">
    <title>Kurs HTML</title>  
    <style type="text/css">
      p {
          color: blue;
          font-family: 'Arial';
          font-size: 50px;
        }
    </style>
</head>
<body>
    <p>To jest przykład akapitu ostylowanego z sekcji head</p>
</body>
</html>
```
###Osadzanie w osobnym pliku
Osobny plik style.css

wówczas html:
```html
<!doctype html>
<html>
<head>
    <meta charset="utf-8">
    <meta name="description" content="Tutaj jest opis!">
    <title>Kurs HTML</title>    
    <link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
<p>To jest przykład akapitu ostylowanego inline</p>
</body>
</html>
```
##Typy selektorów
###Tag - wszystkie elementy danego typu
```html
p {color : black}
<p> Paragraf </p>
```
###Klasa - różne elementy, które są danej klasy
```html
.wazny {color : blue}
<p clas="wazny"> Paragraf </p>
```
###Identyfikator - konkretne identyfikatory
```html
#superważny {color : red}
<p id="superwazny"> Paragraf </p>
```
Można je łączyć np.
```html
p, .wazny {color : blue}
```
Selektor złożony
```html
#news #lead .lead-container p.wazny {color : blue; }
```

##Specyficzność CSS
```html
inline > <head> > .css 
#identyfikator > .klasa > tag
```
##Box model
- el. liniowe - box jest wielkości tekstu
- el. blokowe - box jest maksymalnej szerokości ograniczony kontenerem nadrzędnym
- height x width - wielkość kontenera
- padding - odległość od krawędzi kontenera
- border - ramka
- margin - odstęp kontenera od innych elementów, marginesy nakładają się na siebie,
czyli jako odległość zostaje przyjęty większy margines. Może być ujemny.
- total = content + padding + border + margin
- można zmienić tę właściwość na total = content + padding + border:
```html
box-sizing: border-box
```
- margin: 20px auto -> box będzie na środku kontenera











