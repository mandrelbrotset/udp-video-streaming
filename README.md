# udp-video-streaming
Stream video from one computer to another using OpenCV and UDP sockets in Python.

# how to use
1. Set the ```host``` variable in ```server.py``` to the IP address of the computer running the client program.
2. Run ```> python3 udp_client.py```
3. Run ```> python3 udp_server.py```

Once the server starts, a window will pop up to show the video stream.

# how it works
OpenCV is used to grab a frame from a webcam. The frame is encoded as a jpeg to reduce its size. The encoded frame is sent to the Raspberry Pi over UDP sockets. The Client program on the Raspberry Pi receives the frame, decides it and shows it in an OpenCV window. The process is repeated to create a video stream.

# credits
Credits to GitHub user [chenxiaoqino](https://github.com/chenxiaoqino) as this project was inspired by their CPP version.
https://github.com/chenxiaoqino/udp-image-streaming/
