#  Lær micro:bit - NeoPixel LED

## Steg 1 

Last ned dette programmet til micro:biten og se hva som skjer med LED-lyslenken

```template
let strip = neopixel.create(DigitalPin.P8, 64, NeoPixelMode.RGB)
strip.setPixelColor(0, neopixel.colors(NeoPixelColors.Blue))
strip.setPixelColor(1, neopixel.colors(NeoPixelColors.Green))
basic.forever(function () {
    strip.rotate(1)
    strip.show()
    basic.pause(100)
})
```

## Steg 2 @showdialog
Denne blokken forteller micro:biten at vi har koblet til 64 NeoPixel-lys på Pin 8 (Den blå ledningen)
```blocks
let strip = neopixel.create(DigitalPin.P8, 64, NeoPixelMode.RGB)
```




```ghost
basic.showNumber(0)
basic.showLeds(`
    . . . . .
    . . . . .
    . . . . .
    . . . . .
    . . . . .
    `)
basic.showIcon(IconNames.Heart)
basic.showString("Hello!")
basic.pause(100)
strip.showRainbow(1, 360)
strip.showColor(neopixel.colors(NeoPixelColors.Red))
strip.show()
strip.setPixelColor(0, neopixel.colors(NeoPixelColors.Red))
strip.rotate(1)
basic.forever(function () {
	
})


```


> Åpne denne siden på [https://broccolisurprise.github.io/lr-microbit---neopixel-led/](https://broccolisurprise.github.io/lr-microbit---neopixel-led/)

## Bruk som utvidelse

Dette kodeområdet kan bli lagt til som en **utvidelse** i MakeCode.

* åpne [https://makecode.microbit.org/](https://makecode.microbit.org/)
* klikk på **Nytt prosjekt**
* klikk på **Utvidelser** i menyen under tannhjulet
* søk etter **https://github.com/broccolisurprise/lr-microbit---neopixel-led** og importér

## Rediger dette prosjektet ![Build status badge](https://github.com/broccolisurprise/lr-microbit---neopixel-led/workflows/MakeCode/badge.svg)

For å redigere dette kodeområdet i MakeCode.

* åpne [https://makecode.microbit.org/](https://makecode.microbit.org/)
* klikk på **Importer** og så på **Importér URL**
* lim inn **https://github.com/broccolisurprise/lr-microbit---neopixel-led** og klikk på importér

## Blocks preview

This image shows the blocks code from the last commit in master.
This image may take a few minutes to refresh.

![A rendered view of the blocks](https://github.com/broccolisurprise/lr-microbit---neopixel-led/raw/master/.github/makecode/blocks.png)

#### Metadata (brukes for søk, visualisering)

* for PXT/microbit
<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
