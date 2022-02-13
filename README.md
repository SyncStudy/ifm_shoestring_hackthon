In our solution based on plotly, dash and influxdb, the user will firstly generate the specifications for different robots, and then a wide range of interactive visualizations for different machines for machine power, machine cost, and total cost based on the energy time and total energy getting dynamically from sensors. If a threshold is met, the alert email is generated for further operation.


## Introduction
`dash-manufacture-spc-dashboard` is a dashboard for monitoring read-time process quality along manufacture production line. 
This is a demo of Dash interactive Python framework developed by [Plotly](https//plot.ly/).

## Screenshots
![initial](img/Screen_Shot.png)

## Screencast
![Animated](img/screencast.gif)

## Built With
* [Dash](https://dash.plot.ly/) - Main server and interactive components 
* [Plotly Python](https://plot.ly/python/) - Used to create the interactive plots
* [Dash DAQ](dashdaq.io) - styled technical components for industrial applications

## Requirements
We suggest you to create a separate virtual environment running Python 3 for this app, and install all of the required dependencies there. Run in Terminal/Command Prompt:

```
git clone https://github.com/plotly/dash-manufacture-spc-dashboard.git
cd dash-manufacture-spc-dashboard/
python3 -m virtualenv venv
```
In UNIX system: 

```
source venv/bin/activate
```
In Windows: 

```
venv\Scripts\activate
```

To install all of the required packages to this environment, simply run:

```
pip install -r requirements.txt
```

and all of the required `pip` packages, will be installed, and the app will be able to run.


## How to use this app

Run this app locally by:
```
python app.py
```
Open http://0.0.0.0:8051/ in your browser, you will see a live-updating dashboard.

Click on **Learn more** button to learn more about how this app works.

## What does this app shows

Click on buttons in `Parameter' column to visualize details of trendline on the bottom panel.

Click 'Start' button, trends are updated every two seconds to simulate real-time measurements. The Sparkline on top panel and Control chart on bottom panel show Shewhart process control using mock data. Data falling outside of control limit are signals indicating 'Out of Control(OOC)', and will 
trigger alerts instantly for a detailed checkup. 

Before measurements, operators may config specification parameters for selected process line(metrics).

## Resources and references
* [Shewhart statistical process control](https://en.wikipedia.org/wiki/Shewhart_individuals_control_chart)
* [Dash User Guide](https://dash.plot.ly/)
