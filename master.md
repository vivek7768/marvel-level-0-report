# TASK 1: 3D Printing

## **Objective**
* **Fundamentals:** Understand FDM printer mechanics, STL file structure, and slicing (Cura/Creality).
* **Settings & SOPs:** Master bed temp, infill density, and safety protocols.
* **Execution:** Slice a community STL and initiate a successful print.

### Types of 3-D printing
### 1. Fused Deposition Modeling (FDM)
* **Mechanism:** Melts a thermoplastic filament and extrudes it through a heated nozzle, depositing material layer-by-layer.
* **Common Materials:** PLA (beginner-friendly), ABS (impact resistant), and PETG (weather resistant).
* **Best For:** Functional prototypes, household tools, and low-cost hobbyist projects.
* **Support Structure:** Requires physical "towers" or "lattices" to support overhanging parts, which must be removed manually.
* **Key Characteristic:** Most affordable and accessible method, though it often has visible layer lines on the final part.

### 2. Stereolithography (SLA)
* **Mechanism:** Uses a UV laser to selectively cure (harden) liquid photopolymer resin in a vat, building parts upside down.
* **Common Materials:** Standard resins, "Tough" resins for engineering, and flexible resins.
* **Best For:** Highly detailed miniatures, jewelry masters, and dental applications.
* **Post-Processing:** Prints must be washed in Isopropyl Alcohol (IPA) and then cured further under a UV lamp.
* **Key Characteristic:** Produces extremely smooth surfaces and fine details that are nearly impossible to achieve with FDM.

### 3. Selective Laser Sintering (SLS)
* **Mechanism:** A high-power laser fuses (sinters) small particles of polymer powder into a solid structure.
* **Common Materials:** Primarily Nylon (PA11 or PA12) and occasionally flexible TPU powders.
* **Best For:** Durable end-use parts, complex mechanical assemblies, and interlocking pieces.
* **Design Freedom:** Since the part is surrounded by powder, no dedicated support structures are needed, allowing for hollow or nested geometries.
* **Key Characteristic:** Highly efficient for industrial "batch" printing where dozens of parts can be stacked in a single build volume.

### **PLA 3D Printing: Core Guide & Troubleshooting**

**Material & Setup**
* **Temp/Bed:** Target 200°C–210°C for nozzle; 50°C–60°C for bed to ensure stable adhesion.
* **Cooling/Speed:** Use 100% fan speed for crisp detail; 55mm/s is the quality "sweet spot."

**Environment & Care**
* **Storage:** Store in airtight containers with desiccant; dry at 60°C if filament becomes brittle.
* **Setup:** Avoid drafts; keep enclosures open for PLA to allow for necessary rapid cooling.

**Slicer Optimization**
* **Retraction:** Set 1–5mm (based on drive type) to prevent stringing and oozing.
* **Adhesion:** Use Brims or Rafts for small contact points; ensure a 15s minimum layer time.
* **Extrusion:** Adjust Flow Rate in 5% steps if experiencing over-extrusion or sloppy layers.

**Post-Processing**
* **Finishing:** Join with Superglue; use wet sanding (400–1000 grit) and primer for smoothness.

**Troubleshooting**
* **Adhesion/Warping:** Level bed manually; clean with IPA; lower bed temp if "Elephant’s Foot" occurs.
* **Print Quality:** Increase retraction for stringing; reduce fan speed if layers split or are weak.
![](https://github.com/vivek7768/marvel-level-0-images/blob/e1bd9e69c43ec84798bc9755176dca100a506ec3/ditto.jpeg)
---

# Task 2: API

## Objective
Learn what an API is and how it works. Using any API of your choice, build a user interface.

An **API (Application Programming Interface)** is like a digital waiter. 

* **The Request:** You ask for something.
* **The API:** It takes your request to the kitchen (the server or database).
* **The Response:** It brings the data back to your table

## Project Summary: Country Finder

### Key Features Implemented

* **Dynamic Fetching:** The app doesn't use a saved list; it talks to a live server to get the latest country data every time you search.
* **Smart Search:** It uses a search button to trigger the request and pulls the exact text typed into the input field.
* **Error Handling:** I added a `catch` block to show a helpful message if the country name is wrong or the box is left empty.
* **Responsive Design:** The layout uses a clean card style that centers itself on the screen and works well on different devices.
* **Live Data Display:** The app automatically shows the flag, capital, continent, population, and currency once the data is found.
* **Number Formatting:** I used `toLocaleString()` to make large population numbers easy to read with commas.

### Key Learnings

* **Connecting to APIs:** I learned how to use `fetch()` to get real-time data from an external website.
* **Handling Wait Times:** I practiced using `.then()` to make sure the app waits for the data to load before trying to show it.
* **Fixing Layouts:** I learned how to use CSS to keep images (like flags) at the right size so they don't break the design.
* **Updating the Page:** I mastered using `.innerHTML` to automatically show new country information on the screen.
* **Error Messages:** I added a "catch" to show a helpful message if a country doesn't exist.

![Country Finder](https://github.com/vivek7768/marvel-level-0-images/blob/ca4005a98e94664c4442083566083397f549adc4/api.png)
---
# Task 3: Working with GitHub

## Objective
Familiarize yourself with GitHub integrated workflows such as GitHub Actions, Issues, and pull requests

### Key Learnings: Git & GitHub Workflow
* **Local Environment:** Learned to use **Git Bash** to interact with a local repository via command line rather than a GUI.
* **The Forking Workflow:** Understood that to contribute to a project I don't own, I must first **Fork** it to my own account to gain "Write" permissions.
* **Remote Management:** Learnt the use of `git remote add origin` to link a local folder to a specific GitHub URL.
* **Branching Strategy:** Learned to create isolated **Feature Branches** using `git checkout -b` to keep the `main` branch clean and stable.
* **The Git Lifecycle:** Practiced the standard cycle of making changes, **Staging** (`git add`), **Committing** (`git commit`), and **Pushing** (`git push`).
* **Collaborative Tools:** * Used **GitHub Issues** to document bugs.
    * Opened a **Pull Request (PR)** to propose code changes.
    * Used **Closing Keywords** (e.g., `Closes #1`) to automate issue management.
* **CI/CD Awareness:** Observed how **GitHub Actions** automatically runs test scripts to verify code logic before a merge is allowed.
---
# Task 4: Command Line on Ubuntu

## **Objective**
Get familiar with the command line on Ubuntu by completing given tasks.

### Learning Summary
* **Environment Setup**: Successfully installed WSL2 and initialized an Ubuntu distribution.
* **File System Navigation**: Learned the use of `cd` to navigate directories and `ls` to view contents.
* **Efficient Folder Management**: Used `mkdir` for single folders and **brace expansion** `{1..n}` for bulk creation of 2,600 directories.
* **File Manipulation**:
    * `touch`: Created empty files without needing a text editor.
    * `echo >`: Streamed text directly into new files to quickly populate data.
    * `cat`: Combined and displayed multiple file contents directly in the terminal.
* **Windows Integration**: Utilized `explorer.exe .` to bridge the gap between the Linux kernel and Windows File Explorer.
* **CLI Proficiency**: Developed a foundational understanding of the command-line interface, moving away from reliance on a Graphical User Interface (GUI).

![](https://github.com/vivek7768/marvel-level-0-images/blob/bc02d9863ebf1341262492ebd6f9201cdcac011a/ubuntu1.png)
---
![](https://github.com/vivek7768/marvel-level-0-images/blob/bc02d9863ebf1341262492ebd6f9201cdcac011a/ubuntu2.png)
---

# Task 5 : Build Your Own Brain -Linear Regression from Scratch

## **Objective**
Dive into the core of machine learning by implementing Linear Regression from scratch using , and compare its performance with the scikit-learn implementation. Use the California Housing dataset to evaluate your model on real-world data.

### **Learnings**
* **The Basic Equation:** I learned that at its core, predicting a value is just a simple line equation: $y = mx + b$.
* **Weight and Bias:** I learned how to initialize a weight ($m$) and a bias ($b$) and update them as the "brain" learns.
* **Manual Gradient Descent:** I learned that a model "learns" by checking its error and using calculus to adjust its parameters until the error is at its lowest possible point.
* **Feature Scaling:** I discovered that changing data to center around 0 (Standardization) is essential. It prevents the math from "breaking" and helps the model find the best fit much faster.
* **Model Comparison:** By running my custom code alongside Scikit-Learn, I proved that my manual "scratch" logic produces similar mathematical results as professional tools.
* **Performance Metrics:** I learned how to use $R^2$ to measure success. In this dataset, I found that income explains roughly 47% of the house price variance.
* **Visualization:** I learned how to plot a "Line of Best Fit" to visually confirm that the model has successfully captured the trend of the data.

![](https://github.com/vivek7768/marvel-level-0-images/blob/e1bd9e69c43ec84798bc9755176dca100a506ec3/linear_regression.png)
---
# Task 6 : The Matrix Puzzle — Decode with NumPy & Reveal the Image

## **Objective**
Get hands-on with NumPy and Matplotlib by solving a visual puzzle. 

### **Methodology**
1.  **Loading**: Used `np.load()` to import the `encoded_array.npy` binary data.
2.  **Reshaping**: Converted the initial shape $(200, 50)$ into a square $(100, 100)$ grid to align the pixels based on the total element count ($10,000$).
3.  **Transposing**: Swapped the rows and columns using the `.T` attribute to fix the "sideways" orientation.
4.  **Flipping**: Applied `np.flip(matrix, axis=0)` to correct the vertical orientation (vertical mirror) to ensure the logo was upright.
5.  **Visualization**: Utilized `plt.imshow()` with the `magma` colormap to render the numerical values as a clear visual plot.

![](https://github.com/vivek7768/marvel-level-0-images/blob/e1bd9e69c43ec84798bc9755176dca100a506ec3/matrix.png)
---

### **Key Learnings**

* **Handling Binary Data**: I learned that `.npy` files are specialized binary formats for NumPy and cannot be read as standard text; they require a Python interpreter to "translate" the numbers.
* **Spatial Reasoning with Arrays**: I developed a better understanding of how a flat sequence of numbers maps to a 2D coordinate system (rows and columns).
* **Coordinate Systems in Images**: I discovered that computer images often have different origin points (top-left vs. bottom-left), which is why functions like `np.flip` are essential for correcting "upside-down" data.

---

# Task 7: Create a Portfolio Webpage

## **Objective**
Create a website to showcase your portfolio, including information about yourself, interests, projects, and social media profiles.

### Technical Outcomes
* **Semantic HTML5 Architecture:** Developed a structured document using semantic tags (`<header>`, `<main>`, `<section>`, `<nav>`) to ensure accessibility and better SEO indexing.
* **CSS3 Visual Identity:** Implemented a high-contrast aesthetic using a dark-mode palette (`#0d1117`) with deep red accents (`#990000`) to reflect a professional technical brand.
* **Responsive Layout Design:** Leveraged **CSS Flexbox** and **Grid** to create a layout that adapts to different screen sizes, ensuring the project cards and contact grid remain readable on both mobile and desktop.
* **Navigation Logic:** Integrated internal page linking using `id` attributes and `scroll-behavior: smooth`, providing a seamless user experience (UX) without page reloads.

### Core Learnings
* **UI/UX Principles:** Learned how to use visual hierarchy (font weights, red accent borders, and letter spacing) to guide the reader's eye toward critical information like project titles and contact details.
* **Static Site Optimization:** Understood the benefit of building a lightweight, static site without unnecessary JavaScript to ensure near-instant load times on all networks.
* **Front-End Organization:** Gained experience in separating concerns by keeping structural content in `index.html` and design logic in `style.css`, making the codebase easier to maintain and update.
* **Professional Branding:** Practiced translating complex engineering projects (like LiFi and Radar systems) into concise, high-impact descriptions suitable for recruiters or project leads.

![](https://github.com/vivek7768/marvel-level-0-images/blob/6088c77c634a3763399342c45ac1bb7638a7c36d/portfolio1.png)
---
![](https://github.com/vivek7768/marvel-level-0-images/blob/6088c77c634a3763399342c45ac1bb7638a7c36d/portfolio2.png)

---

# Task 8: Writing Resource Article Using Markdown

## Ovrview

*Unmanned Aerial Vehicles (UAVs)* are transforming agriculture by enabling **high-resolution spatial intelligence** and *automated farm operations*. Beyond simple aerial imaging, modern agricultural UAV systems integrate **advanced sensing**, *geospatial analytics*, **artificial intelligence (AI)**, and autonomous flight control. These capabilities support *precision livestock monitoring*, **soil assessment**, crop modeling, and automated input delivery.

This article explores the **technical architecture**, operational workflows, advanced sensing technologies, system integration models, and emerging innovations in *UAV-enabled smart farming*.

---

## 1. UAV-Driven Smart Farming Systems

Unlike traditional farming practices that rely on manual inspection and uniform field treatment, *UAV-enabled smart farming* uses **spatial data** and automation to make targeted decisions at *sub-field resolution*.

Modern agricultural UAV operations typically involve:

- **Autonomous flight planning**
- *Real-time telemetry*
- **Sensor fusion**
- Edge or cloud-based data analytics
- Integration with *farm management software*

This ecosystem enables **data-driven agriculture** rather than experience-based estimation.

---

## 2. Core Applications of UAVs in Agriculture

### 2.1 Livestock Monitoring and Management

UAVs equipped with *RGB and thermal sensors* are used to:

- Track herd movement  
- Detect injured or isolated animals  
- Monitor body temperature for *early disease detection*  
- Locate animals across large grazing areas  

**Thermal anomaly detection** can identify potential health issues before visible symptoms appear.

---

### 2.2 Soil Condition and Erosion Mapping

UAV-based photogrammetry and *LiDAR* allow for:

- **High-resolution terrain modeling**
- Drainage pattern identification  
- Soil erosion risk assessment  
- Field leveling optimization  

*Digital Elevation Models (DEMs)* generated from UAV data help design irrigation layouts and prevent nutrient runoff.

---

### 2.3 Crop Growth Modeling

By collecting periodic aerial data, UAVs support *time-series analysis* of crop development. Growth rate modeling allows farmers to:

- Detect uneven emergence  
- Monitor canopy expansion  
- Estimate biomass accumulation  
- Forecast yield variability  

Vegetation indices such as **NDVI** and **EVI** are computed using spectral reflectance data:

---

## 3. Advanced Technologies in Agricultural UAV Systems

### 3.1 Sensor Fusion

Modern UAV platforms combine multiple sensors simultaneously:

| Sensor Type     | Function                          |
|----------------|-----------------------------------|
| Multispectral  | Crop stress detection             |
| Thermal        | Water stress and livestock health |
| LiDAR          | Terrain and canopy structure      |
| RGB            | Visual inspection                 |

**Sensor fusion** enhances accuracy by correlating multiple data layers.

---

### 3.2 Autonomous Navigation and Swarm Coordination

Advanced UAV systems incorporate:

- **RTK GNSS positioning** (±2–3 cm accuracy)  
- Obstacle avoidance sensors  
- *Autonomous waypoint navigation*  
- Multi-drone *swarm coordination*  

Swarm systems allow multiple UAVs to divide large farms into segments, significantly reducing mission time.

---

### 3.3 Edge Computing

Instead of uploading all imagery to cloud servers, some UAVs process data onboard using *embedded GPUs*. This allows:

- **Real-time crop stress alerts**
- Immediate spraying decisions  
- Reduced data transmission requirements  

*Edge analytics* minimizes latency between detection and action.

---

## 4. Data Workflow Architecture

A typical UAV agricultural workflow includes:

1. **Mission Planning**
   - Define geofence boundaries  
   - Set altitude and overlap  
   - Upload flight path  

2. **Autonomous Data Collection**
   - Execute grid or adaptive flight  
   - Capture geo-referenced imagery  

3. **Data Processing**
   - Orthomosaic generation  
   - Radiometric correction  
   - Vegetation index computation  

4. **Decision Support Integration**
   - Upload maps to farm management system  
   - Generate treatment prescriptions  
   - Deploy ground or aerial application systems  

This structured workflow ensures **operational efficiency** and *data consistency*.

---

## 5. Operational Efficiency Metrics

### Coverage and Performance

| Parameter              | Typical Value     |
|------------------------|------------------|
| Coverage per flight    | 50–200 hectares  |
| Flight time            | 25–60 minutes    |
| Spatial resolution     | 2–5 cm/pixel     |
| RTK accuracy           | ±2 cm            |

### Efficiency Gains

- **60–80% reduction** in manual scouting time  
- *10–20% fertilizer optimization*  
- 15% improvement in irrigation efficiency  
- Faster response to disease outbreaks  

---

## 6. Implementation Challenges

Despite technological progress, UAV deployment in agriculture faces several barriers:

### 6.1 Regulatory Constraints
Airspace restrictions and licensing requirements vary by region and can limit operational flexibility.

### 6.2 Data Complexity
High-resolution mapping produces *large datasets* requiring advanced storage infrastructure and analytics expertise.

### 6.3 Environmental Factors
Wind speed, rainfall, and cloud cover can affect **data accuracy** and flight stability.

### 6.4 Economic Barriers
Initial setup costs include:

- UAV platform  
- Sensors  
- Processing software  
- Operator training  
- Maintenance  

Small-scale farms may require *cooperative ownership models* to reduce cost burden.

---

## 7. Emerging Innovations

### 7.1 AI-Based Disease Detection

**Deep learning models** trained on aerial imagery can automatically classify crop diseases and pest infestations.

### 7.2 Automated Seeding Drones

Experimental UAVs are being developed to:

- Plant cover crops  
- Reseed damaged zones  
- Perform reforestation in degraded land  


## 8. Sustainability Impact

UAV-enabled farming contributes to:

- Reduced chemical runoff  
- Lower fuel consumption compared to ground machinery  
- Optimized water usage  
- Reduced soil compaction  

These benefits align with **sustainable agriculture** and *climate-resilient farming practices*.

---

## 9. Conclusion

*UAV-based smart farming* represents a significant advancement in agricultural technology. By combining **autonomous flight systems**, multisensor data acquisition, *AI-driven analytics*, and integrated decision support, UAVs enable farmers to optimize productivity while minimizing environmental impact.

Although challenges such as regulatory compliance, data management, and capital investment remain, continued advancements in **autonomy**, *artificial intelligence*, and cost reduction are accelerating adoption. In the coming years, UAV systems are expected to become a foundational component of digitally connected, **data-driven agricultural ecosystems**.

---

# TASK 9:TINKERCAD

## OBJECTIVE
Create a Tinkercad account and familiarize yourself with the application. 

1. **Distance Estimation:** Simulate a simple circuit using an ultrasonic sensor to estimate the distance between an obstacle and the sensor.
2. **Serial Monitoring:** Display the results on the serial monitor. 
3. **Radar System:** Create a radar system using an ultrasonic sensor and servo motor to detect objects within a certain range.

---

## OUTCOMES

### Components Used:
* **Arduino Uno R3**
* **Ultrasonic Sensor (HC-SR04)**
* **Servo Motor**

### Circuit Image
![](https://github.com/vivek7768/marvel-level-0-images/blob/7b0b424e23e611b1bac14c24e5c48a646c320dfe/tinker1.png)

---

### Circuit Connections
![](https://github.com/vivek7768/marvel-level-0-images/blob/7b0b424e23e611b1bac14c24e5c48a646c320dfe/tinker2.png)

---
## Working Principle of an Ultrasonic Sensor

The ultrasonic sensor (like the common HC-SR04) operates on the **Sonar (Sound Navigation and Ranging)** principle, using sound waves to measure the distance to an object. Here is the process in four points:

1. **Triggering the Pulse:**
   The sensor is activated when a microcontroller sends a short 10µs pulse to the **Trigger pin**. This tells the sensor to emit a series of eight ultrasonic "chirps" at a frequency of 40 kHz, which is beyond the range of human hearing.

2. **Sound Wave Propagation:**
   These sound waves travel through the air at the speed of sound (approximately 340 m/s). If there is an object in their path, the waves hit the surface and **reflect back** toward the sensor as an echo.

3. **Echo Detection:**
   The sensor's receiver (the "ear") detects the returning sound waves. Upon receiving the echo, the **Echo pin** on the sensor goes HIGH. It stays HIGH for the exact duration it took for the sound to travel to the object and back.

4. **Distance Calculation:**
   The microcontroller measures the time the Echo pin remained HIGH. Since the speed of sound is constant, the distance is calculated using the formula:
   $$Distance = \frac{Time \times Speed\ of\ Sound}{2}$$
   *(The result is divided by 2 because the sound traveled to the object and back).*

## Working Principle of a Servo Motor

The servo motor operates on a **Closed-Loop Feedback System**, ensuring high precision in angular positioning. Here is the process broken down into four points:

1. **Pulse Width Modulation (PWM) Signal:**
   The motor receives a control signal from a microcontroller. The **width of the pulse** (duration) determines the target angle of the output shaft. Usually, a 1.5ms pulse centers the motor at 90°, while 1ms and 2ms pulses represent 0° and 180° respectively.

2. **Internal Feedback (Potentiometer):**
   The output shaft is connected to an internal **potentiometer** (a variable resistor). As the motor rotates, the potentiometer's resistance changes, providing a voltage signal that tells the control circuit the exact current position of the shaft.

3. **Error Detection (Comparator):**
   An internal control circuit compares the target position (from the PWM signal) with the actual position (from the potentiometer). If there is a difference between the two, an **"error signal"** is generated.

4. **Correction and Holding:**
   The error signal triggers the internal DC motor to rotate in the direction that reduces the error. Once the shaft reaches the desired position, the error signal becomes zero, and the motor stops and holds that position firmly.

## WHAT I LEARNT

* **Circuit Prototyping:** Gained hands-on experience in making digital connections and utilizing basic electronic components within the Tinkercad environment.
* **Component Integration:** Successfully learnt the working principles and interfacing of the **Arduino Uno**, **Ultrasonic Sensor**, and **Servo Motor**.
* **Logic & Coding:** Developed an understanding of how to translate physical movements into code using Pulse Width Modulation and the speed of sound constants.

---

# Task 10: Speed Control of DC Motor

## Objective
To interface a DC motor with an Arduino UNO using the **L298N H-Bridge motor driver** to achieve variable speed control through Pulse Width Modulation (PWM) and understand the logic required for motor activation and braking.

### Methodology
Followed a modular approach to bridge high-current hardware with low-power microprocessing:

1.  **H-Bridge Logic Configuration:** Using two digital pins (`input1`, `input2`) to establish the direction of current. Setting one `HIGH` and the other `LOW` creates the potential difference needed for rotation.
2.  **PWM Speed Regulation:** Utilizing the `enablePin` (Pin 9) on the Arduino. By using `analogWrite()`, the Arduino sends a square wave signal. The speed is determined by the **Duty Cycle**:
    * **Low Speed:** 80/255 (approx. 31% duty cycle)
    * **Medium Speed:** 150/255 (approx. 58% duty cycle)
    * **Full Speed:** 255/255 (100% duty cycle)
3.  **Signal Isolation:** The L298N acts as an intermediary, taking the 5V logic signals from the Arduino and switching a separate power source to the motor, protecting the Arduino from high current draws.

---
![](https://github.com/vivek7768/marvel-level-0-images/blob/cfcff8e9a6a8bb3c4a5621cab6a37b26c2fd1cc6/dc_circuit.png)

### Outcomes
* **Variable Speed Execution:** Successfully demonstrated four distinct motor states (Slow, Medium, Full, and Stop) in a continuous loop.
* **Static Friction Observation:** Identified that the motor requires a minimum PWM threshold (starting at 80) to overcome "stiction" (static friction) and begin spinning.
* **Voltage Drop Awareness:** Noticed that the motor receives slightly less than the input voltage due to the internal resistance of the L298N's Darlington transistors.
* **Real-time Monitoring:** The Serial Monitor successfully synced physical motor movement with code execution, providing a debugging trail for speed transitions.

https://github.com/user-attachments/assets/e9c8f861-f775-4dec-9601-01f39c2930bd

### Learning Points
* **The H-Bridge Mechanism:** Learned that the L298N uses four switches (transistors) in an "H" configuration. Closing two specific switches allows current to flow one way; closing the other two reverses it. **Crucially, closing all four would cause a short circuit, which the L298N logic prevents.**
* **Current Sourcing Limits:** Learned that an Arduino cannot power a motor directly from its I/O pins due to current limitations (max ~40mA), necessitating the L298N driver which can handle up to 2A.
* **PWM vs. Analog:** Gained an understanding that `analogWrite` is a "faked" analog signal created by pulsing a digital signal on and off rapidly. The motor "averages" these pulses into a smooth rotation.
* **Common Grounding:** Learned the "Golden Rule" of electronics: the Arduino GND and the L298N GND must be connected to ensure a common reference point for logic signals, even if they use different power supplies.

---

# Task 11: LED Toggle Using ESP32

## Objective
To design and deploy a web server using the ESP32 to control GPIO pins via a browser-based interface over a local Wi-Fi network.

### Methodology

* **Hardware:** ESP32 board, two LEDs connected to GPIO 26 and 27.
* **Network:** Utilized `WiFi.h` to connect the ESP32 to a local Access Point.
* **Protocol:** Configured a `WiFiServer` on Port 80 to listen for HTTP GET requests.
* **Logic:** The code parses the HTTP header using `header.indexOf()` to detect specific URL paths and toggles the corresponding `digitalWrite()` states.
* **UI:** Served a custom HTML/CSS page to the client to provide interactive buttons.

### Outcomes
* **Connectivity:** Successfully established a stable Wi-Fi connection and assigned a local IP.
* **Web Control:** Remote devices on the same network successfully toggled LEDs.
* **Stability:** Implemented a 2-second timeout to handle disconnected clients effectively.
* **Visuals:** The UI dynamically reflects the "ON/OFF" state using CSS classes.

https://github.com/user-attachments/assets/e77327a1-e4dc-4bda-bc8a-cc7ec44b09a3

### Learning
* **Embedded Networking:** Gained hands-on experience with the TCP/IP stack on microcontrollers.
* **Request Handling:** Learned to parse raw HTTP streams into actionable logic.
* **State Management:** Managed synchronized states between physical hardware and a digital UI.
* **Web Design:** Applied basic CSS within C++ `client.print` statements for mobile responsiveness.

---
# Task 12: Soldering Prerequisites

## Objective
The primary goal of this project was to transition from temporary breadboard prototyping to permanent circuit assembly. Specifically:

---

## Learning Outcomes
Upon completion of this project, the following competencies were achieved:
* **Tool Proficiency:** Demonstrated correct use of the soldering iron, solder wire.
* **Thermal Management:** Learned to balance heat application—long enough to melt solder into the joint, but quick enough to avoid heat-damaging the LED or lifting the copper pad.
* **Visual Inspection:** Gained the ability to distinguish between a "Good Joint" (shiny, concave cone) and a "Fail" (cold joint or solder bridge).

---

## Key Learnings & Observations

### Safety & Best Practices
* **Fume Awareness:** Using rosin-core solder creates smoke; I learned the importance of working in a well-ventilated area or using a fume extractor.
* **Tip Maintenance:** I discovered that a "tinned" (silver-looking) iron tip transfers heat significantly better than a dark, oxidized tip.
* **Mechanical Stability:** Bending the leads at a 45-degree angle on the bottom of the perf board is essential for keeping components flush against the board while flipping it over to solder.

![](https://github.com/vivek7768/marvel-level-0-images/blob/3017f2183a74e5f7476d2392ffc69719284ee7ae/Solder.jpeg)
---

# Task 13: Design a 555 Astable Multivibrator

## Objective
To design and assemble a **555 IC Astable Multivibrator** on a breadboard that produces a square wave with a **60% duty cycle**, and to verify the resulting waveform's timing and shape using a **Digital Storage Oscilloscope (DSO)**.

---

## Outcomes
* **Successful Hardware Build:** A functional pulse-generator circuit assembled on a breadboard.
* **Signal Visualization:** Real-time observation of the charging/discharging cycle on the DSO.
* **Accuracy Check:** Confirmation that the high-to-low ratio of the wave matches the 60% design target.
* **Steady 5V Pulse:** A reliable 5V output signal generated from the RPS (Regulated Power Supply).

---
![](https://github.com/vivek7768/marvel-level-0-images/blob/0e3b9f2fa69be6ad8b20838fba21581042d81a5a/555.jpeg)

## Learnings
* **Breadboard Proficiency:** Learned how to translate a schematic into a physical circuit layout.
* **DSO Operation:** Mastered how to trigger, scale, and measure pulse width and frequency on an oscilloscope.
* **Formula Application:** Understood how the ratio of $R_1$ and $R_2$ directly controls the "On" vs "Off" time of the signal.
* **Real-world Testing:** Observed how physical component tolerances (resistor/capacitor variations) affect the theoretical 60% goal.

---
# Task 14: Active Participation

### Objective
To participate in a technical event and apply problem-solving skills using AI tools.

### Reverse Prompt Engineering | Impetus 26.0 (CTRL + Z)
Participated in a specialized challenge focused on the mechanics of Large Language Models. 

* **Objective:** Analyzed complex AI-generated outputs to reconstruct the exact prompts required to replicate them.
* **Key Learnings:** Gained a deep understanding of how prompt architecture, constraints, and stylistic cues influence model behavior.
* **Outcome:** Improved practical skills in prompt optimization and black-box model analysis.
---
# Task 15: Introduction to VR

Virtual Reality is a technology that uses computer-generated images which are displayed directly through a head-mounted display on our eyes, giving us a full immersive experience. The user can give inputs through controllers that fit in both hands.

---

## Comparison: VR vs. AR

The following table highlights the fundamental differences between these two transformative technologies:

| Feature | Virtual Reality (VR) | Augmented Reality (AR) |
| :--- | :--- | :--- |
| **Environment** | Completely digital/artificial; shuts out the physical world. | Overlays digital data onto the real-world physical environment. |
| **Hardware** | VR Headsets (e.g., Meta Quest 3, HTC Vive), controllers. | Smartphones, Tablets, AR Glasses (e.g., Xreal, Apple Vision Pro). |
| **User Presence** | User is "somewhere else." | User remains grounded in the "here and now." |
| **Motion Tracking** | Requires 6 Degrees of Freedom (6DoF) to track movement in space. | Relies on SLAM (Simultaneous Localization and Mapping) to anchor objects. |
| **Bandwidth** | High; requires low latency to prevent motion sickness. | Moderate; focuses on data overlay and camera processing. |

---

## The Technology Stack

The development of immersive experiences relies on powerful software engines that handle physics, lighting, and real-time rendering:

* **Unity:** The leader for cross-platform mobile and standalone XR. It utilizes the **Data-Oriented Technology Stack (DOTS)** to handle thousands of interactive objects simultaneously.
* **Unreal Engine 5.5:** Considered the gold standard for photorealism. It uses **Lumen** (dynamic lighting) and **Nanite** (virtualized geometry) to stream cinema-quality visuals directly to headsets.

---

## The Indian XR Ecosystem

India has successfully transitioned from being a "back-office" for XR to becoming a global hub for high-end industrial and educational solutions.

### Key Indian Players:

* **CHRP-INDIA:** A global leader in industrial safety. They gained international recognition for implementing the world’s first VR safety training modules specifically designed for live coal and ore mines.
* **TCS (Tata Consultancy Services):** Leveraging its **"XR-as-a-Service,"** TCS builds massive metaverse environments for global retail brands and handles immersive employee onboarding for Fortune 500 companies.
* **AjnaLens:** Known for their **AjnaXR** headsets, they focus on "human intelligence augmentation," providing AR/VR tools specifically for vocational training and the defense sector.
* **Tiltlabs:** Specializes in **Virtual Production** and gamified enterprise solutions, effectively bridging the gap between blockchain technology and immersive experiences.
* **Quidich Innovation Labs:** A pioneer in using AR for live sports broadcasting (notably Cricket), overlaying real-time player stats and graphics onto live drone feeds to enhance the viewer experience.

---
# **Aviation Domain-Specific Tasks**
---
## 1. History of Aviation

![](https://github.com/vivek7768/marvel-level-0-images/blob/3b6c493454aa7a1acd1ba48e7726c46de17ff90b/aviation_flowchart_.png)

## 2. Introduction to Flight Simulators


### Section 1: The RadioMaster TX16S MKII Controller

The **TX16S MKII** is a high-end transmitter that uses the EdgeTX operating system. In a simulator environment, it acts as a high-precision HID (Human Interface Device) to translate physical stick movements into digital commands.

### 1.1 RC Channel Assignment
Standard drone configurations generally follow the **AETR** (Aileron, Elevator, Throttle, Rudder) channel mapping:

* **Channel 1 (Roll / Aileron):** Controlled by the horizontal movement of the right stick. It tilts the drone left or right.
* **Channel 2 (Pitch / Elevator):** Controlled by the vertical movement of the right stick. It tilts the drone forward or backward.
* **Channel 3 (Throttle):** Controlled by the vertical movement of the left stick. It manages the total RPM of the motors to control altitude.
* **Channel 4 (Yaw / Rudder):** Controlled by the horizontal movement of the left stick. It rotates the drone on its center vertical axis.

### 1.2 Simulator Connection & Hardware Setup
To interface the TX16S MKII with the **Real Drone Racing** application:

1.  **USB Interface:** Connect the radio to the PC using the **top USB-C port**. When prompted on the radio's screen, select **"USB Joystick (HID)"**.
2.  **Software Calibration:** Within the simulator, each axis must be calibrated so the software recognizes the "dead center" and the maximum travel limits (typically 1000µs to 2000µs) of the gimbals.

---

## Section 2: Quadcopter Dynamics and Motor Mixing

A quadcopter changes its position in 3D space by varying the thrust of individual motors. This process is managed by a "Motor Mixer" within the flight controller.

### 2.1 Motor Mixing Logic (X-Configuration)
In a standard quadcopter layout, two motors rotate clockwise (CW) and two rotate counter-clockwise (CCW) to cancel out rotational torque.

| Maneuver | Motor Speed Adjustment | Physical Result |
| :--- | :--- | :--- |
| **Throttle Up** | All motors (1, 2, 3, 4) increase speed equally. | Vertical Lift / Climb |
| **Pitch Forward** | Front motors (1 & 2) decrease; Rear motors (3 & 4) increase. | Nose dips, forward movement. |
| **Roll Right** | Left motors (1 & 4) increase; Right motors (2 & 3) decrease. | Drone tilts to the right. |
| **Yaw Clockwise** | CCW motors (1 & 3) increase; CW motors (2 & 4) decrease. | Torque imbalance rotates the frame. |

![](https://github.com/vivek7768/marvel-level-0-images/blob/b87ce0d3b83311ab834df860a89cccc908bb13c4/drone.jpeg)

### 2.2 Mechanical Coordination
To maintain a specific path in the simulator, the pilot must coordinate these mixing behaviors. For example, a **Coordinated Turn** requires a simultaneous input of both **Roll** and **Yaw** in the same direction. This ensures the drone "carves" through the air rather than sliding laterally (drifting) while maintaining the desired heading.

---

## 3. Flying the Airblock Drone

### Objective: To learn about and operate the Airblock Drone available in the lab.

### 1. Operation & Control
* **Application:** The drone is operated via the **Makeblock App**, which supports both manual remote control and block-based graphical programming (similar to Scratch).
* **Connectivity:** Bluetooth-enabled for real-time control and coding.


### 2. Propulsion System
* **Motor Type:** **6 x Coreless DC Motors**. These provide the necessary RPM for a modular hexacopter while remaining lightweight.
* **Propellers:** * Plastic blades housed within protective hexagonal frames.
    * Configuration includes both **Clockwise (CW)** and **Counter-Clockwise (CCW)** propellers to maintain flight stability.
    * **Safety:** The enclosed design makes the propellers safe for indoor use and beginner pilots.
 
  
![](https://github.com/vivek7768/marvel-level-0-images/blob/66a6c22755ba8fab45cee071e596e59554e9436a/airblock2.webp)

---

### 3. Physical Construction & Modular Design
* **Material:** **EPP (Expanded Polypropylene) Foam**. This is a closed-cell foam known for being:
    * **Lightweight:** Crucial for flight efficiency.
    * **Flexible & Durable:** Absorbs impacts without breaking.
    * **Solid:** Maintains structural integrity across different forms.
* **Assembly:** Features **Magnetic Connectors** for tool-free, modular transformation. This magnetized system allows for rapid assembly and disassembly.

### Modular Configurations
The Airblock's modularity allows it to take several specialized shapes:
* **Drone:** A standard hexacopter configuration for aerial flight.
* **Hovercraft:** Utilizes the foam's buoyancy and motor thrust to glide over flat ground or water.
* **Triangle/Spider:** Creative DIY configurations that demonstrate the versatility of the magnetized blocks for land-based movement or unique flight physics.

---
![](https://github.com/vivek7768/marvel-level-0-images/blob/9c1199c53326a942adf2ea37ac8bdbe76ecc7c41/airblock1.webp)

---

## 4. Battery & Power
* **Type:** Lithium Polymer (**LiPo**) battery.
* **Voltage:** 7.4V.
* **Capacity:** Typically **700mAh**.
* **Performance:** * **Flight Time:** Approximately 6 minutes.
    * **Hovercraft/Land Time:** Approximately 16 minutes.
    * **Charging Time:** 60–90 minutes via USB.

---

## 5. Onboard Sensors
* **Ultrasonic Sensor:** For altitude hold and detecting distance from the ground.
* **Barometer:** Monitors air pressure to assist in height stabilization.
* **6-axis Gyroscope:** Ensures orientation and balance across all modular forms.

---




