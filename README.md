# Harry's Toolbox

Harry's Toolbox is a collection of lightweight Python utilities. Each designed
to simplify a basic task, such as calculating the framerate of a video feed.

## FPS Counter

The FPS Counter module is designed to simplify the process of monitoring the
framerate of a video feed.

After creating an instance of the FPSCounter class, the module works by
expanding "to string" function `__str__` to measure the time since the `__str__`
function was last called, and uses this time difference to calculate the frame
rate.

### Example Usage

```python
import time

from harrys_toolbox import FPSCounter

fps = FPSCounter()

while True:

    # Prints out the framerate of the video
    print(fps)

    # Delay to represent the processing time of each frame.
    time.sleep(0.01)

```

### Terminal Output

```
FPS: 96.02
```
