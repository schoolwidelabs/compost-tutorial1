# Compost Tutorial
Text for tutorial

```template
basic.forever(function () {
    basic.showNumber(0)
})
```

## Step 1
When you turn the micro:bt on, ``||gatorEnvironment: initialize||`` the environmental sensor

```blocks
gatorEnvironment.beginEnvironment()
```

```ghost
input.onButtonPressed(Button.A, function () {
    basic.showNumber(Math.round(gatorEnvironment.getMeasurement(measurementType.humidity)))
})
```

## Step 2 
When you turn the micro:bt on, ``||gatorLog: initialize||`` the data logger sensor

```blocks
gatorLog.begin()
```

## Step 3
``|Download your code|`` and try it out


```package
gatorEnvironment=github:sparkfun/pxt-gator-environment
gatorSoil=github:sparkfun/pxt-gator-soil
gatorLog=github:sparkfun/pxt-gator-log
gatorRTC=github:sparkfun/pxt-gator-RTC
```
