---
layout: post
lang: pl
title:  Obiekt Application i jego bezczynność
list-icon: "/assets/images/posts/cat-idle.jpg" 
date: 2019-01-11 10:32:34 +0100
categories: delphi vcl tapplication
---
Wszyscy programiści Delphi doskonale znają obiekt `Application`. Zazwyczaj programiście wystarcza świadomość istnienia takiego obiektu. Dzisiaj przyjrzę się stanowi bezczynności tego obiektu. Dlaczego? Ponieważ od jego działania zależy działania całej naszej aplikacji. Głębsza wiedza na ten temat pozwali świadomiej wykorzystywać możliwości platformy VCL. 

# Eksperyment z obrazkiem

To jest test z lewej strony: Wszyscy programiści Delphi doskonale znają obiekt `Application`. Zazwyczaj programiście wystarcza świadomość istnienia takiego obiektu. Dzisiaj przyjrzę się stanowi bezczynności tego obiektu. 

```pascal
type
  /// <summary> TStoper - counting time passed </summary>
  TStoper = class(TComponent)
  private
    FStartTick: Cardinal;
    function GetEnlapsedMs: Integer;
  published
    procedure Reset;
    function IfPassThenReset (TimeToPassMs: Integer): boolean;
    property EnlapsedMs: Integer read GetEnlapsedMs;
  end;

procedure TStoper.Reset;
begin
  if self.Name = 'Object1WithElements' then
    FStartTick := 0;
  FStartTick := WinAPI.Windows.GetTickCount;
end;

function TStoper.GetEnlapsedMs: Integer;
begin
  Result := abs(WinAPI.Windows.GetTickCount - FStartTick);
end;

function TStoper.IfPassThenReset(TimeToPassMs: Integer): boolean;
begin
  Result := false;
  Result := EnlapsedMs>TimeToPassMs;
  if Result then
    Reset;
end;
```

[![Śpiący kotek]({{ page.list-icon | relative_url }})](aaa)

A to jest tekst z prawej strony: Dlaczego? Ponieważ od jego działania zależy działania całej naszej aplikacji. Głębsza wiedza na ten temat pozwali świadomiej wykorzystywać możliwości platformy VCL. 

To jest test z lewej strony: Wszyscy programiści Delphi doskonale znają obiekt `Application`. Zazwyczaj programiście wystarcza świadomość istnienia takiego obiektu. Dzisiaj przyjrzę się stanowi bezczynności tego obiektu. 
