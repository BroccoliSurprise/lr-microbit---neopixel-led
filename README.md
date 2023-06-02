#  Lær micro:bit - NeoPixel LED

## Steg 0 @showdialog
Denne blokken forteller micro:biten at det er 64 NeoPixel-lys koblet til på Pin 8 (Den blå ledningen)
```blocks
let strip = neopixel.create(DigitalPin.P8, 64, NeoPixelMode.RGB)
```


## Steg 1 - Test

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

## Steg 2 - Lek
Prøv å lage dine egne fine fargemønster. Klarer du å lage en regnbue som beveger seg?


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
