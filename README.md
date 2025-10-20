# 🤖 AI Object Detection Web App

## 👋 About the Project

This project is a client-side web application designed for real-time AI object detection directly within your web browser. It leverages your device's camera to identify various objects in its field of view, powered by a pre-trained machine learning model. The application aims to provide an accessible and interactive way to experience on-device AI capabilities with a straightforward user interface.

### ✨ Features

*   **Real-time Object Detection**: Processes your device's camera feed to detect objects in real-time.
*   **Toggle AI Functionality**: Easily switch the object detection AI on or off as needed.
*   **Adjustable Frame Rate**: Control the detection processing speed with a dedicated FPS slider, allowing for performance optimization on different devices.
*   **Dynamic Resolution Scaling**: Automatically adjusts the video stream resolution to fit the display size effectively.
*   **Camera Permission Handling**: Includes robust logic for gracefully handling camera access requests and providing user feedback.
*   **Loading Indicators**: Displays clear status messages while the AI model loads or awaits camera permission.

### 🚀 Technologies Used

*   **HTML5, CSS3, JavaScript**: The foundational web technologies for structuring content, styling, and enabling interactivity.
*   **ml5.js**: A high-level, user-friendly machine learning library for the web, specifically utilizing the `COCO SSD` model for object detection.
*   **Materialize CSS**: A responsive front-end framework based on Google's Material Design, used for enhancing UI components and overall aesthetics.

### 🖼️ Screenshots

<a href="https://ibb.co/JCNgfJr"><img src="https://i.ibb.co/3kwQDZS/preview-combined.jpg" alt="preview-combined" width="100%"></a>

## ⚙️ Getting Started

To get a copy of this project up and running on your local machine, follow the instructions below.

### Prerequisites

*   A modern web browser (e.g., Chrome, Firefox, Edge) with camera access permissions enabled.
*   Git installed on your system.

### Installation

1.  **Clone the repository:**
    bash
    git clone https://github.com/your-username/ai-object-detection.git # Replace with your actual repository URL
    cd ai-object-detection
    

### Running Locally

This is a static web application, meaning it doesn't require a backend server for its core functionality. You can serve it using any simple HTTP server.

1.  **Using Python's built-in HTTP server:**
    Open your terminal in the project's root directory and execute:
    bash
    python -m http.server 8000
    
    Then, open your web browser and navigate to `http://localhost:8000`.

2.  **Using `live-server` (recommended for development):**
    If you have Node.js and npm installed, you can install `live-server` globally:
    bash
    npm install -g live-server
    
    Navigate to the project root directory in your terminal and run:
    bash
    live-server
    
    This will automatically open the application in your default browser and provide live reloading on file changes.

## 🚀 Usage

Once the application is loaded in your browser and has successfully obtained camera access, you will see a live video feed from your device's camera.

1.  **Initial Load**: The application will initially display "Loading..." or "Waiting for camera permission" until the AI model is fully ready and camera access is granted.
2.  **AI Toggle**:
    *   Locate the "AI" toggle switch. Once enabled, flip it to "On" to activate real-time object detection. Detected objects will be highlighted with bounding boxes and labels overlaid on the video feed.
    *   Flip it to "Off" to temporarily pause AI processing and view the raw camera feed without detections.
3.  **Frame Rate (FPS) Slider**:
    *   Use the "FPS" range slider to adjust the frequency at which the AI processes frames from the video stream.
    *   **Higher FPS**: Provides a smoother detection experience but consumes more CPU resources, potentially affecting performance on less powerful devices.
    *   **Lower FPS**: Reduces CPU usage, making it suitable for devices with limited processing power, though detections may appear less frequent.

### 🌐 Browser Support

The application has been tested and confirmed to work on the following browsers:

| Browser           | Supported |
| :---------------- | :-------- |
| Firefox           | ✅        |
| Chrome            | ✅        |
| Edge              | ✅        |
| Internet Explorer | ❌        |

| Mobile Browser | Supported |
| :------------- | :-------- |
| Firefox        | ✅        |
| Chrome         | ✅        |

### ✨ Try it

If you'd like to try out a live version of the application without any local setup, you can access the demo here:
[https://woody.pizza/tensorflow/object-detection/](https://woody.pizza/tensorflow/object-detection/)

### 🙏 Credits

*   **Materialize**: For providing the responsive and visually appealing UI components.
*   **ml5.js**: For simplifying the integration of machine learning models into web applications, making AI accessible on the web.
*   **github-readme-generator**: For generate README.md file.
