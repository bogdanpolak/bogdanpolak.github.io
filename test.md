---
layout: post
title: Przykładowy testowy wpis na bloga
date: 2018-07-01 15:00
---

Test formatowania wpisów oraz sprawdzenie stylów wprowadzanych w dokumentach `Markdown`. Każdy wpis na blogu to nowy dokument `md`, który trzeba odpowiednio sformatować. Możliwości formatowania są bardziej ograniczone w typowych dokumentach `HTML`. Jednak są to możliwości wystarczające do napisania ciekawego i atrakcyjnie sformatowanego artykułu.

# Nagłówek H1 (tytuł wpisu)

## Nagłówek H2

### Nagłówek H3

#### Nagłówek H4

---

## Łącza

Łącze do szablonu Jekyll'a [Jekyll Now](http://github.com/barryclark/jekyll-now/)

Długie, pełne łącze HTTP: <https://github.com/bogdanpolak/spring-demos>
  
## Obrazy

Paragraf nad obrazkiem: Litwo! Ojczyzno moja! Ty jesteś jak zdrowie, Ile cię trzeba cenić, ten tylko się dowie, kto cię stracił. Dziś piękność twą w całej ozdobie widzę i opisuję, bo tęsknię po tobie. Matka Boska, Panno święta, co Jasnej bronisz Częstochowy i w Ostrej świecisz Bramie!  Ty, co gród zamkowy Nowogródzki ochraniasz z jego wiernym ludem! Jak mnie dziecko do zdrowia powróciłaś cudem.

[![Opis obrazka - logo generatora Jekyll]({{ "/assets/images/posts/jekyll-logo.png" | relative_url }} "an image title")](/assets/images/posts/Jekyll__Logo_Full.png)
(kliknij na obrazek aby go powiększyć) Test poniżej obrazka: Litwo! Ojczyzno moja! Ty jesteś jak zdrowie, Ile cię trzeba cenić, ten tylko się dowie, kto cię stracił. Dziś piękność twą w całej ozdobie widzę i opisuję, bo tęsknię po tobie. Matka Boska, Panno święta, co Jasnej bronisz Częstochowy i w Ostrej świecisz Bramie!  Ty, co gród zamkowy Nowogródzki ochraniasz z jego wiernym ludem! Jak mnie dziecko do zdrowia powróciłaś cudem ... 

## Listy

* Lista wyliczeniowa (*)
- Lista wyliczeniowa, składnia alternatywna (-)
+ Lista wyliczeniowa, inna alternatywa (+)
* Poziom 1 listy
  * poziom drugi listy
    * poziom trzeci

1. Lista numerowana
1. Druga pozycja numerowana
1. Trzecia pozycja
    1. pod-pozycja pierwsza drugiej pozycji
1. Czwarta pozycja
    * poziom 2 lista wyliczeniowa
    * druga pozycja wyliczeniowa
1. Piąta pozycja


## Style tekstu

Tekst pisany kursywą: _Litwo! Ojczyzno moja! Ty jesteś jak zdrowie, Ile cię trzeba cenić, ten tylko się dowie, kto cię stracił. Dziś piękność twą w całej ozdobie widzę i opisuję, bo tęsknię po tobie._

Tekst wytłuszczony (pogrubiony): **Matka Boska, Panno święta, co Jasnej bronisz Częstochowy i w Ostrej świecisz Bramie!  Ty, co gród zamkowy Nowogródzki ochraniasz z jego wiernym ludem! Jak mnie dziecko do zdrowia powróciłaś cudem.**

Kod w tekście: `procedure code() begin end` ... trochę zwykłego tekstu: Litwo! Ojczyzno moja! Ty jesteś jak zdrowie, Ile cię trzeba cenić, ten tylko się dowie, kto cię stracił.

## Cytaty

> Wisława Szymborska:  
> Czytanie książek to najpiękniejsza zabawa, jaką sobie ludzkość wymyśliła  
>> Alan Alexander Milne – Kubuś Puchatek:
>> - A jeśli pewnego dnia będę musiał odejść? - spytał Krzyś, ściskając Misiową łapkę. - Co wtedy?
>> - Nic wielkiego. - zapewnił go Puchatek. - Posiedzę tu sobie i na Ciebie poczekam. Kiedy się kogoś kocha, to ten drugi ktoś nigdy nie znika.


## Linie poziome oddzielające

Linie można dodawać korzystając z potrójnej gwiazdki (*) lub potrójnego myślnika (-):

---
***

## Formatowanie kodu

Syntax highlighting can be used by wrapping your code in a liquid tag like so:

```pascal
procedure TForm1.FormCreate(Sender: TObject);
begin
  ReportMemoryLeaksOnShutdown := True;
  OnFormReady := procedure(Sender: TObject)
    begin
      with TButton.Create(Self) do
      begin
        AlignWithMargins := True;
        Align := alTop;
        Caption := 'Button Jeden';
        Parent := GroupBox1;
      end;
    end;
end;
```
 
```pascal
// Komentarz Delphi
{ Drugi komentarz }
(* Trzeci komentarz *)

procedure TForm1.Button1Click(Sender: TObject);
begin
    Button1.Caption := 'Kliknęto';
end;
```
 
## Inne znaki formatujące

Use two trailing spaces  
on the right  
to create line break tags  
 
