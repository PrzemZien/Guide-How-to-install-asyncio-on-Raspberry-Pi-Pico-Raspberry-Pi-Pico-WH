# Guide-How-to-install-asyncio-on-Raspberry-Pi-Pico-Raspberry-Pi-Pico-WH

First, create lib folder in you CIRCUITPY(D:)

![alt text](Images/1.png)


![alt text](Images/2.png)

Then download adafruit bundle with libraries for Circuitpython:

[(https://circuitpython.org/libraries)](https://circuitpython.org/libraries)


![alt text](Images/3.png)


After downloading it, open the zip folder then open libaries and locate asyncio and adafruit_ticks.mpy: 

![alt text](Images/4.png)

![alt text](Images/5.png)

![alt text](Images/6.png)

To check if asyncio is installed correctly, you can create a simple test script: 

`import asyncio

async def test():
    print("Asyncio is working!")
    await asyncio.sleep(1)
    print("Done!")

asyncio.run(test())`
