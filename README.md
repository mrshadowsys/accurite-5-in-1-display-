# AcuRite 5-in-1 Receiver with Arduino Nano
A few months ago when i started winter sailing in the Pacific , i came across a need 
every time i radioed my wife on the shore , she had to run downstairs to look at our display and talk me over the radio the wind speed and direction on shore, we needed a seccond display , so after playing with Jens Jensen code ,so i added a i2c display. 
It shows the Wind Speed in both KMph and Knots , so its easy to read to both landlubbers and sea people alike.


This project is a simple yet effective Arduino Nano-based receiver for decoding weather data from the AcuRite 5-in-1 sensor suite, which transmits using 433 MHz OOK modulation. The received data is processed and displayed on a 16x2 LCD screen via I2C.
Key Features

    Supports AcuRite 5-in-1 sensors for:

        Wind speed

        Wind direction

        Temperature (°C)

    433 MHz OOK Receiver compatible

    16x2 I2C LCD Display outputs:

        Wind speed in km/h and knots

        Wind direction in degrees and compass heading

        Ambient temperature in Celsius

    Lightweight interrupt-driven decoder with CRC validation

    Efficient LCD updates every second

    Compact and low-power friendly

How It Works

    The system captures OOK pulses using an interrupt on pin D2.

    It synchronizes to the pulse stream, reconstructs bits, and stores them in a buffer.

    A CRC check ensures data integrity.

    When a valid message is received, the data is parsed into readable metrics:

        Wind speed is scaled and converted from raw sensor values to km/h and knots.

        Wind direction is mapped to degrees and compass points.

        Temperature is decoded from Fahrenheit and converted to Celsius.

    A 16x2 LCD displays updated values once per second.

Data Output Example (LCD)

12.6km/h  6.8knt
270° W   T 23°C
