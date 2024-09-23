# Saker jag fixade på min code

## Issue #1
( a ) får inte vara en child av ( ul )

Så här såg det utt först

~~~ html
    <nav>
        <ul class="navbar">
            <a href="index.html">Home</a>
            <a href="om.html">Om oss</a>
            <a href="bilder.html">Bilder</a>
            <a href="bob.html">bob</a>
        </ul>  
    </nav>
~~~

Den klagade på att ul fanns men det var a i den så ifall jag tar bort ul och flytar classen till nav så funkar det som jag vill.


så här ser det ut efter jag fixade problemet
 ~~~ html
    <nav class="navbar">
        <!--<ul >-->
            <a href="index.html">Home</a>
            <a href="om.html">Om oss</a>
            <a href="bilder.html">Bilder</a>
            <a href="bob.html">bob</a>
        <!--</ul> a får inte vara under ul--> 
    </nav>
 ~~~
 Jag bara kommenterade bort ul så jag skulle komma ihåg det till nu.

 ## Issue #2
( li ) får inte vara en child av ( body )


Så här såg den ut först, tog bort lite av texten för att det var så mycket text
~~~ html
    
<a>Allergier: En av de mest påtagliga vanliga<a> 
<li>Ekosystemet: Björkarna spelar en viktig nektar</li>
<li>Landskapsbilden: När björkarna blommar miljö för invånarna</li>
<li>Kulturell Betydelse: Björkarna har som firar naturens återfödelse, där björkarna spelar en central roll.</li>
<h3> björkarnas blomning </h3>
</body>
~~~
Den klagar på att li finns i body ensam.
För att fixa detta så är det bara att läga till ul i li. Eftersom att jag glömnde bort varför detta skulle fixas så kan jag inte svara på den


Det jag ialla fall ändrade var att läga till ul och ge den en class, classen är odefenierad eftersom att det inte finns en class som heter "lista"
 ~~~ html
    
     <a>Allergier: En av de mest påtagliga vanliga<a> 
     <ul class="lista">
        <li>Ekosystemet: Björkarna spelar en viktig nektar</li>
    
        <li>Landskapsbilden: När björkarna blommar miljö för invånarna</li>
    
        <li>Kulturell Betydelse: Björkarna har som firar naturens återfödelse, där björkarna spelar en central roll.</li>
        <!-- li får inte vara i body-->
     </ul>
    <h3> björkarnas blomning </h3>
</body>
~~~

## Inga mer problem 



