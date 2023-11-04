# CS-4800 Project S.H.E.R.L.O.C.K.
**S**erver **H**ealth and **E**mpirical **R**eal-time **L**atency for **O**nline **C**onnection **K**nowledge

This program is designed for California State University Stanislaus' CS-4800 2023 Fall class with Dr. Hatem. It is meant to be able to ping servers to check to see if they are up (responsive) or if they are down (unresponsive), alongisde the latency between connections. The program will ping based on a user given, or predetermined, polling rate. The status of the server, and its latency, is then saved to a database alongside a timestamp which will be used later to display a histogram of each indvidual server's statuses.  This program is hostable on a local machine, yet accessible through the web assuming firewalls permit, and will require an internet conneciton to be useful. However, it is also capable of pinging device on a Local Area Network (LAN) and Wide Area Network (WAN) if the user desires.

## Team Members
- Christian Alameda
- Anthony Castillo
- Sierra Pangilinan
- Vel Perez-Barba

## Capabilities
- Runs locally
- Accept user given IP addresses, domain names, and/or websites
- Stores given IP addresses in a database
- Polls those addresses every (user defiend elapsed period) and stores latency, downtime, and uptime info
- Display an uptime/downtime and/or latency histogram
- A webui for user interactions with the program
- Can trace connections to see where the connection ends if it is unable to reach its destination. (WIP)

### Disclaimer
- All aspects are subject to change as the project progresses.

#### Explanation of Folders and Files.
- client: Contains the main python file which connects all the controllers together and communicates to the server on behalf of the controllers.
- controllers: Python files which host the individual controllers for our project.
- server: Python files responsible for facilitating communication between the database and the client(s).
- static: Holds a folder of images and a folder of css files.
- templates: Holds a collection of html files that import from the static pictures and css folders.
- exampleCode: Just some exploration on how things work and give a shot to some things.
- oldFiles: Temporary Storage of old files.
- start.py: The single file which initializes the core of our project.
