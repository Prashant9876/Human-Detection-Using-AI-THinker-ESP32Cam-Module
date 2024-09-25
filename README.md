# Human-Detection-Using-AI-THinker-ESP32Cam-Module
An Arduino-compatible library for real-time person detection using the Ai Thinker ESP32 CAM module. Integrates OpenCV and YOLO models for edge AI processing, perfect for automation in smart homes, security, and energy-saving projects. Simple setup and deployment with Arduino IDE.


# ESP32 Ai Thinker CAM Person Detection Arduino Library

This is an Arduino-compatible library for **real-time person detection** using the **Ai Thinker ESP32 CAM module**. The library integrates with **OpenCV** and **YOLO** models to bring efficient AI-based person detection capabilities into your IoT and automation projects.

## Features
- **Real-time person detection** using the ESP32 Ai Thinker CAM module.
- Supports **OpenCV** and **YOLO** object detection models.
- Ideal for **automation** tasks such as smart homes, security, and more.
- Easily integrated with **Arduino IDE** for simple deployment.

## Hardware Requirements
- **Ai Thinker ESP32 CAM** module
- USB to TTL Serial Adapter (for programming)
- FTDI or equivalent USB-to-Serial converter
- Jumper wires

## Software Requirements
- Arduino IDE
- ESP32 Board Package (for Arduino IDE)
- Ai Thinker ESP32 CAM module library

## Getting Started

### Step 1: Download and Install the Library
1. Download the library from the [GitHub repository](https://github.com/your-repo-link).
2. Open the Arduino IDE.
3. Navigate to **Sketch** > **Include Library** > **Add .ZIP Library...**.
4. Select the downloaded `.zip` file and click **Open**. This will install the library in your Arduino IDE.

### Step 2: Install the ESP32 Board Package
1. Open Arduino IDE, go to **File** > **Preferences**.
2. In the "Additional Boards Manager URLs" field, add the following URL:  
   `https://dl.espressif.com/dl/package_esp32_index.json`
3. Go to **Tools** > **Board** > **Boards Manager**.
4. Search for "ESP32" and install the latest version of the **ESP32 by Espressif Systems** package.

### Step 3: Setup the Ai Thinker ESP32 CAM
1. Connect the **ESP32 CAM module** to your computer using the USB-to-TTL Serial Adapter.  
   - Connect the **5V** pin of the adapter to **VCC** of the ESP32 CAM module.
   - Connect **GND** to **GND**.
   - Connect **TX** of the adapter to **U0R** of the ESP32 CAM module.
   - Connect **RX** to **U0T**.
   - Short the **GPIO0** pin to **GND** for flashing.

### Step 4: Uploading the Program
1. In the Arduino IDE, go to **Tools** > **Board** and select **ESP32 Wrover Module**.
2. Under **Tools** > **Partition Scheme**, select **Huge APP (3MB No OTA)**.
3. Choose the correct **COM Port** for your USB adapter.
4. Load an example sketch for person detection from the library:  
   `File` > `Examples` > `ESP32_CAM_PersonDetection`.
5. Click **Upload** to upload the code to the ESP32 CAM module.
6. After uploading, disconnect **GPIO0** from **GND**, then press the **Reset** button on the ESP32 CAM to start the program.

### Step 5: Running the Program
1. Once the program is uploaded, the ESP32 CAM will start detecting persons in real-time.
2. The data can be viewed through the serial monitor or via the web server hosted on the ESP32 CAM (IP address will be displayed in the serial monitor).

## Contributions
Feel free to contribute by creating a pull request or raising an issue in this repository.

## License
This project is licensed under the MIT License.

## Contact
For any questions or suggestions, feel free to reach out to me at [your-email@example.com].

