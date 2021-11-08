# jetson_ros2_workspace
A template for ROS2 development and deployment on NVIDIA Jetson

Enable Docker Default Runtime:
- Add ```"default-runtime": "nvidia" ``` to your ```/etc/docker/daemon.json``` ``` $ vi /etc/docker/daemon.json```
    ``` 
    {
        "runtimes": {
            "nvidia": {
                "path": "nvidia-container-runtime",
                "runtimeArgs": []
            }
        },
        "default-runtime": "nvidia"
    }
    ```
- Restart docker or Reboot system ``` $ sudo systemctl restart docker```