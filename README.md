# ros-html

Here are some html files to help you to integrate ROS to your web pages.

## Installation
#### Step 1
Install rosbridge suite for your ROS distribution
```sh
sudo apt-get install ros-melodic-rosbridge-suite
```

#### Step 2
clone this repo on your computer
```sh
git clone https://github.com/Kramoth/ros-html.git
```
## Usage
Before opening any html file launch rosbridge server:
```sh
roslaunch rosbridge_server rosbridge_websocket.launch
```
### Subscriber
#### step 1
Open on your web browser subscriber.html
#### step 2
Open the web browser's console verify that the connexion between the rosbridge server and the web page is done.
If not verify that you had launch the web server or if the port setup has not been changed.
#### step 3
Open a terminal then:
```sh
rostopic pub /listener std_msgs/String "data: 'hello'"  
```
Check on the web browser console if the message "hello" has been received.

















