<div align="center">

# 🎮 ROS Web Joystick Teleop

**Lightweight browser joystick for driving any ROS robot from a phone.**

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![ROS](https://img.shields.io/badge/ROS-22314E?style=for-the-badge&logo=ros&logoColor=white)

</div>

---

## ✨ Features

- **Touch joystick** (nipplejs) → `geometry_msgs/Twist` on a configurable topic (default `/cmd_vel`)
- **Emergency stop** — publishes an e-stop message and sends repeated zero-velocity commands
- **Configurable telemetry cards** — choose topic, message type and field path at runtime
  (defaults: battery `/battery_state`, temperature `/system/temperature`, fan `/system/fan_rpm`)
- **Auto rosbridge address** — connects to `ws://<page-host>:9090` by default, so serving the page from the robot just works

## 🚀 Getting Started

```bash
# robot
ros2 launch rosbridge_server rosbridge_websocket_launch.xml

# this app
npm install
npm run dev -- --host     # open from your phone on the same network
```

## 🛠️ Tech Stack

React · Vite · roslib · nipplejs

---

<div align="center">
Built by <a href="https://github.com/Bariscompeng">Barış Coşkun</a>
</div>
