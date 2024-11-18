# BumbleBoard

BumbleBoard is an FRC dashboard using React and TypeScript developed by BumbleB 3339. This dashboard provides a customized, interactive interface for controlling and monitoring an FRC robot. It includes multiple widgets, such as live camera streams, graphs, indicators, etc, helping teams have a real-time overview of their robot's performance.

---

## 📚 Table of Contents

1. [About](#about)
2. [Installing](#installing)
3. [Connecting to your robot](#connecting-to-your-robot)
4. [Adding widgets](#adding-widgets)
   - [Widget List](#widget-list)
     - [Number](#number)
     - [Slider](#slider)
     - [Graph](#graph)
     - [Boolean Indicator](#boolean-indicator)
     - [Switch](#switch)
     - [Text Indicator](#text-indicator)
     - [Chooser](#chooser)
     - [Camera](#camera)
     - [Field](#field)
     - [Timer](#timer)
     - [Table](#table)
5. [Getting Help](#getting-help)

---

## About

BumbleBoard is designed to give FRC teams a responsive interface for robot control and data visualization. With this dashboard, team members can easily observe real-time data, and control various robot functions from a single location. BumbleBoard is developed to be highly customizable, allowing teams to adapt the dashboard to their specific robot's needs.

## Installing

To get BumbleBoard running, follow these steps to install and run BumbleBoard.

### 1. Download the latest release

Go to the [BumbleBoard GitHub releases](https://github.com/BumbleB3339/BumbleBoard/releases/latest) page and download the latest setup file (EXE) for Windows.

### 2. Run the installer

Open the downloaded setup file and follow the on-screen instructions to install BumbleBoard on your system.

### 3. Launch BumbleBoard

Once installed, you can find BumbleBoard in your Start menu or Applications folder.

## Connecting to your robot

To connect BumbleBoard to your robot, follow these steps:

1. In the top-right corner of the BumbleBoard interface, click the **Settings** button located next to the minimize button.

2. In the Settings panel, locate the `Connect By` field and choose:

   - **Team Number:** BumbleBoard will automatically connect to your robot’s network table using the default IP configuration based on the team number you entered.

   - **IP Address:** If you prefer to specify the robot’s IP address directly, enter the IP address of your robot.

After configuring your connection, BumbleBoard will connect to your robot's network based on your selected settings.

## Adding widgets

To add widgets to BumbleBoard:

1. Open the sidebar by clicking the Sidebar button in the top-left corner of the app, or by pressing Tab on your keyboard.

2. Once the sidebar is open, you’ll see two widget options:

   - NetworkTables: Drag any network table entry from this menu to add it as a widget on the dashboard.
   - Custom Widgets: Drag any custom widget from this menu to add it to the dashboard.

### **Widget list**

#### **Number**

Displays a numeric value. Supports reading and writing to the entry.
<br />
Parameters:

- `Digits After Point`: Number of decimal places to display.
- `Step Type`:
  - **Automatic**: Steps adjust dynamically based on the entry value.
  - **Manual**: Allows setting a step value.

![](/app-pics/NumberWidget.png)

#### **Slider**

Displays a numeric value as a slider. Supports reading and writing to the entry.
<br />
Parameters:

- `Min`: Minimum value of the slider.
- `Max`: Maximum value of the slider.
- `Step`: The step increment for slider movements.

![](/app-pics/SliderWidget.png)

#### **Graph**

Displays values over time. Supports data types such as _int_, _double_, _boolean_, _int[]_, _double[]_, and _boolean[]_. Multiple entries can be displayed in the same graph widget by adding paths using the plus button.
<br />
Parameters: 

- `Min`: Minimum value of the graph. Leave blank for auto-scaling.
- `Max`: Maximum value of the graph. Leave blank for auto-scaling.

![](/app-pics/GraphWidget.png)

#### **Boolean Indicator**

Displays a boolean value with visual feedback using colors.
<br />
Parameters:

- `Color on True`: The color displayed when the value is true.
- `Color on False`: The color displayed when the value is false.

![](/app-pics/BooleanIndicatorWidget.png)

#### **Switch**

Displays a boolean value with a toggle switch. Supports reading and writing to the entry.

![](/app-pics/SwitchWidget.png)

#### **Text Indicator**

Displays a string value along with a visual indicator (color/image) based on the value. Useful for enums or similar cases. Supports reading and writing to the entry.
<br />
Parameters:

- `Indicators`:
  - Add indicators with the plus button.
  - Enter the specific value in the 'value' field.
  - Choose an indicator type (color/image).
  - Select the desired color or image for the indicator.

![](/app-pics/TextIndicatorWidget.png)

#### **Chooser**

Displays a sendable chooser (e.g., Auto Chooser).

![](/app-pics/ChooserWidget.png)

#### **Camera**

Displays a live camera stream from the robot.
<br />
Parameters:

- `Source`: The camera stream to display.

![](/app-pics/CameraWidget.png)

#### **Field**

Displays the robot’s position on the field based on its alliance. For the red alliance, `(0,0)` is the bottom-left corner; for the blue alliance, `(0,0)` is the top-right corner.
<br />
Parameters:

- `Alliance`: Set to **red**, **blue**, or auto-detect from the FMS.
- `History`: Number of "ghost" robots (past positions) shown behind the current position.

![](/app-pics/FieldWidget.png)

#### **Timer**

Displays a timer that reads from an entry.
<br />
Parameters:

- `Blink Time`: Time at which the timer starts flashing red and white.

![](/app-pics/TimerWidget.png)

#### **Table**

Displays multiple entries in a table format. Supports all entry types.

![](/app-pics/TableWidget.png)

## Getting Help

If you need any assistance, we are here to help!

1. Open an issue on our GitHub repository, where we can track and resolve problems efficiently.
2. Alternatively, post your question or concern on Chief Delphi, where other teams and developers can also assist.
3. For direct support, feel free to reach out to us on [Instagram](https://www.instagram.com/bumbleb3339/).

We’re committed to ensuring BumbleBoard works smoothly and effectively for your team!
