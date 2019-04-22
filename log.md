# LinuxFest presentation log

## 4-21-2019

LinuxFest Northwest is next weekend!

I'm breaking the program I wrote into individual components, following the Unix philosophy. I should give an overview of that as well. 

## 4-22-2019

Took screenshots of Bryan Cantrill's slides. I should make a slideshare and put them on it.

[And here it is.](https://www.slideshare.net/BobbyTowers1/unix-141630706)

The *Unix philosophy* according to Doug Mcllroy:

* Write programs that do one thing and do it well
* Write programs to work together
* Write programs that handle text streams, because that is a universal interface

Bryan Cantrill:

> Four decades later, this philosophy remains the single most important revolution in software systems thinking!

Me:

> In case it isn't obvious, I say that this is because it allows our programs to be used in ways beyond that which we intended.

## A tour of music code formats

Make sure to cover:

* Music XML or whatever
* [Alda](https://github.com/alda-lang/alda)/Edna!
* Lilypond/TeX
* [Music Macro Language (MML)](https://en.wikipedia.org/wiki/Music_Macro_Language) looks especially interesting, at least from a historical perspective on 8-bit music. It began in BASIC:

```
 10 TEMPO 4
 20 A$="E5R1E3R0D3R0E3R0E1R0D1R0-G4R1"
 30 B$="F3R0F1R0F1R0A3R0F1R0E1R0D1R0D1R0E5R0"
 40 C$="C3R0C1R0C1R0E3R0C1R0-B1R0C1R0-B1R0-A1R0-A1-B5R0"
 50 D$="E1R0E1R0E1R0E1R0E1R0E1R0D1R0E1R0E1R0E1R0D1R0-A1R0-A1R0B3R1"
 60 E$="-A1R0-B1R0C1R0D1R0E1R0F1R0E1R0F3R1A3R1B1R0A1R0F3R0E3R0E1R0E4R0"
 100 MUSIC A$+B$+B$
 110 MUSIC C$+C$+B$
 120 MUSIC C$+D$+E$
```