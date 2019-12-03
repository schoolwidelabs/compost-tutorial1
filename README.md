# Compost Tutorial

## Step 1
When you turn the micro:bt on, ``||gatorEnvironment: initialize||`` the environmental sensor

```blocks
gatorEnvironment.beginEnvironment()
```

## Step 2 
When you turn the micro:bt on, ``||gatorLog: initialize||`` the data logger sensor

```blocks
gatorLog.begin()
```

## Step 5
``|Download your code|`` and try it out


```template
gatorLog.begin()
gatorLog.openFile("data.csv")
```

```ghost
input.onButtonPressed(Button.A, function () {
    basic.showNumber(Math.round(gatorEnvironment.getMeasurement(measurementType.humidity)))
})
```

```package
gatorEnvironment=github:sparkfun/pxt-gator-environment
gatorSoil=github:sparkfun/pxt-gator-soil
gatorLog=github:sparkfun/pxt-gator-log
gatorRTC=github:sparkfun/pxt-gator-RTC
```
