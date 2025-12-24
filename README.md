# MarioGameOnDocker
Mario Game Deployment On Docker

![image](https://github.com/user-attachments/assets/1062e296-8003-4109-8457-619a64cb462e)

<img width="1864" height="949" alt="image" src="https://github.com/user-attachments/assets/ad74170d-d57f-424d-ac7a-4446f089869e" />

<img width="1919" height="932" alt="image" src="https://github.com/user-attachments/assets/21939c43-3cc3-403a-8226-f4b2b4b7e61b" />


- My Mario Game Docker Image is present here - https://hub.docker.com/r/jinny1/mario-game

## How to Run the Application

1. **Fork & Clone the repository**:
    - Fork the repository https://github.com/sudhanshuvlog/MarioGameOnDocker.git
    - Once you have forked the repo on your github account, Clone the repo in your system
        ```bash
        git clone <your repo URL>
        cd MarioGameOnDocker
        ```

2. **Launch Server**
    - Launch an AWS EC2 Instance with `t2.micro` as Instance Type, and Give atleast 8GB of EBS Volume.
    - In `Security Group` you can allow port no 80 and 22.

3. **Build the Docker image**
   - This command builds a Docker image named mario-game-nginx.
        ```bash
        docker build -t mario-game-nginx .
        ```

4. **Run the Docker container**
    - After building the image, you can run a container using this image with the following command:
        ```bash
        docker run -d -p 80:80 mario-game-nginx
        ```
5.  **Play the Game**
    - To play the game, just hit to `http://<Ec2 instance Public IP >`

7. **Contact**

    For any inquiries or issues, please contact [me](https://www.linkedin.com/in/sudhanshu--pandey/)


