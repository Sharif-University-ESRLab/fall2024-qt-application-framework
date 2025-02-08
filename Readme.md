
![Logo](https://via.placeholder.com/600x150?text=Your+Logo+Here+600x150)


# QT Home
A Qt application and a server to control it on a Raspberry Pi. This project enables seamless interaction between the application and the server, allowing for efficient management and operation on the Raspberry Pi platform.


## Tools
In this section, you should mention the hardware or simulators utilized in your project.
- Qemu
- QT
- Django
- Raspberry Pi 3B


## Implementation Details

The application on the Raspberry Pi was developed using Qt Creator and QML, providing a robust and interactive interface. For communication between the application and the server, we implemented WebSocket, which facilitates real-time data exchange. The server was built using Django along with its specialized libraries, enabling a powerful backend system. It includes a user interface for controlling the Raspberry Pi, ensuring smooth management operations. The connection between the server and the application is maintained through WebSocket, allowing for efficient and seamless interaction.
Additionally, we utilized QEMU to create a customized image for deploying on the Raspberry Pi. This custom image includes all the necessary tools and dependencies required to run the application, streamlining the deployment process and ensuring a ready-to-use environment.

## How to Run
#### Build Image
Download the QT shared libaries and you base image and Run the folloing script to create a custom image
```bash
  bash ./code/build-image.sh
```

#### Run server

For running server you should first install all requirements.

```
pip install -r requirements.txt
```

After that you can run server using this command:

```
daphne -p 8000 server.asgi:application
```


## Related Links
 - [QT](https://qt.io)
 - [qemu](https://www.qemu.org/)
 - [Django Doc](https://docs.djangoproject.com/en/5.0/)


## Authors
- Mahdi Alizadeh
- Nima Najafi
- MohammadHosein Salimi

