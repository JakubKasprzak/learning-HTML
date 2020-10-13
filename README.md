# learning-HTML

###HTML - HyperText Markup Language
Czyli zestaw znacznikiów, które klient (jakaś aplikacja np. przeglądarka) może interpretować i poprawnie wyświetlać

HyperText - bo teksty są interpretowane w ramach protokołu HTTP w przeglądarce  

Markup - bo zawiera znaczniki (tzw. tagi)

Language - może być czytany przez maszynę i człowieka

###Atrybut
+znacznik atrybut="">

np. hiperłącze

+a href="http://google.com" target="_blank"> Link do google +/a> target blank otwiera link w nowym oknie

+a href="#sekcja4"> Przejdź do sekcji 4 +/a> Przenosi do sekcja4 jeśli +section id="sekcja4">S4+/section>

+!-- komentarz -->

+br/> - przenieś do nowej linii

+hr/> - linia pozioma 

+img> src="link do obrazka" alt="tekst alternatywny do obrazka" width="80%" height=""/>

jeśli poda się tylko % w szerokośći ro obrazek będzie skalował się razem z przeglądarką (responsywaność) zachowując proporcje (nie podane height)


##Tagi
[więcej tutaj](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

###Elementy blokowe
- zawsze mają znaczniki otwierające i zamykające
- zajmują całą szerokość dokumentu (można to zmienić w css)

+header> górna sekcja strony 

+footer> stopka 

+p> akapity 

+ul> i +ol> listy nieuporządkowna(kropki) i uporządkowana(numerki)

+h1> fo +h6> nagłówki, dobrze żeby h1 był tylko jeden w dokumencie a h2 nie więcej niż 5

+section> sekcje czyli elementy grupujące części strony

+article> merytorycznie odrębne części strony np. artykuły

+aside> elementy treści jeśli nie ma sensu by mogły być wycięte

+nav> najczęściej linki, któe dobrze jest zawrzeć w elemencie +ul> (lista) a każda pozycja listy +li>

+div> element bez znaczenie semantycznego, pełni rolę organizacyjną

+blockquote> większy element który jest cytatem (np. cały paragraf +p>) 

###Elementy liniowe
- zajmują przestrzeń wymaganą dla ich treści (można to zmienić w css)

+span> element bez znaczenia semantycznego, do wyróżeninia wizualnego

+a> linki 

+em> ważne treści, pochyla, robot ideksujące rozpoznaje je jako słowa kluczowe

+i> pochylone 

+b> bold

+q> cytat zamyka treść w cudzysłowach

+strong> pogrubienie wizualne



