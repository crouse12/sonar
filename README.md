# pxt-sonar [![Build Status](https://travis-ci.org/Microsoft/pxt-sonar.svg?branch=master)](https://travis-ci.org/Microsoft/pxt-sonar)

MakeCode的超音波HC-SR04積木

## Usage

這個積木主要是會回傳感應值  修改自pxt-sonar

```sig
sonar.ping(DigitalPin.P1, DigitalPin.P2, PingUnit.Inches);
```

## Charting the distance

Use the ``plot bar graph`` block to visualize the distance reported by your sensor.

```blocks
basic.forever(() => {
    let p = sonar.ping(DigitalPin.P1, DigitalPin.P2, PingUnit.Inches);
    led.plotBarGraph(p, 0);
})
```

## License
MIT

## Supported targets
* for PXT/microbit
* for PXT/calliope
(The metadata above is needed for package search.)


    ## Code of Conduct

    This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

