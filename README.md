
# Project Title
**Irrigation Data Distribution System**

## Description
This repository contains a Python-based network application that uses both TCP and UDP multicast sockets to distribute data regarding nitrate and phosphate levels within an irrigation system. The project includes four main components:
1. **Server**: Sends irrigation data to connected clients.
2. **Node Receiver 1**: Receives data from the server, processes it, and forwards it via multicast.
3. **Node Receiver 2**: Similar to Node Receiver 1, but operates on different ports and potentially serves a different segment of the network.
4. **Central Node**: Acts as a central hub that receives data from the server and broadcasts updates to multiple receivers.

Each node not only relays data but also performs local computations to determine irrigation actions based on nutrient levels.

## Installation
To get this project running on your local machine, follow these steps:
```bash
# Clone the repository
git clone https://github.com/yourusername/yourprojectname.git
cd yourprojectname

# No additional dependencies are required, as the code uses standard Python libraries.
```

## Usage
To run the system, start each component in a separate terminal window. Ensure your system supports Python's `socket`, `struct`, `sys`, `pickle`, and `time` modules.

```bash
# Terminal 1: Run the server
python server.py

# Terminal 2: Run the first node receiver
python node_receiver1.py

# Terminal 3: Run the second node receiver
python node_receiver2.py

# Terminal 4: Run the central node
python central_node.py
```

Each script corresponds to a separate file in the repository:
- `server.py` for the server.
- `node_receiver1.py` for Node Receiver 1.
- `node_receiver2.py` for Node Receiver 2.
- `central_node.py` for the Central Node.

## Contributing
Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature')
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License
Distributed under the MIT License. See `LICENSE` for more information.

## Contact
Your Name - [your-email@example.com](mailto:your-email@example.com)

## Acknowledgments
- Hat tip to anyone whose code was used
- Inspiration
- etc.
