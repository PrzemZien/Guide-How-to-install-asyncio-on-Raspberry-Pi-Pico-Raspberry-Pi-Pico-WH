# Guide-How-to-install-asyncio-on-Raspberry-Pi-Pico-Raspberry-Pi-Pico-WH

### **Step 1: Create a `lib` Folder in CIRCUITPY**

First, create a `lib` folder in your **CIRCUITPY** drive (D:). 

![alt text](Images/1.png)


![alt text](Images/2.png)

### **Step 2: Download the Adafruit CircuitPython Library Bundle**  

Go to the official CircuitPython library page and download the latest bundle or bundle for your Circuitpython version:  

[(https://circuitpython.org/libraries)](https://circuitpython.org/libraries)


![alt text](Images/3.png)

### **Step 3: Extract and Copy Required files**  

After downloading the ZIP file, open it and navigate to the `lib` folder inside the ZIP file.

Locate the following two files:  
- `asyncio` (folder)  
- `adafruit_ticks.mpy` (file)

![alt text](Images/4.png)


![alt text](Images/5.png)


![alt text](Images/6.png)

Copy **both** the `asyncio` folder and `adafruit_ticks.mpy` file to the `lib` folder on your CIRCUITPY drive.  

Your `lib` folder should now contain: 

![alt text](Images/7.png)

### **Step 4: Verify Installation** 

To check if asyncio is installed correctly, you can create a simple test script: 

```
import asyncio

async def test():
    print("Asyncio is working!")
    await asyncio.sleep(1)
    print("Done!")
asyncio.run(test())
