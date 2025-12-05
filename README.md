<iframe width="560" height="315" 
    src="https://www.youtube.com/embed/LxKLbWbJDBo?si=94jFgAl1I5x0MIGl" 
    title="YouTube video player" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
    referrerpolicy="strict-origin-when-cross-origin" 
    allowfullscreen>
</iframe>

This project is a robotic arm control system run on an ESP32 using the FreeRTOS real-time operating system. It functions through the use of a potentiometer to control movement along the horizontal pivot, with corresponding warning LEDs to indicate when the arm is extended into unsafe areas, such as in the working area of another system on an assembly line. For the second axis of control, two push buttons allow the arm to move a controlled distance forward or backward, with color-coded LEDs indicating when a movement is taking place. Commands are inserted into a queue to ensure all commands are executed at an even pace, even with erratic operator input. The arm's horizontal position, as well as response to command inputs are displays through a UART serial terminal for operator observation. Additonally, there is a heartbeat LED to give a quick indication of system health.