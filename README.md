
 [![MasterHead](https://dotnet.microsoft.com/static/images/games/unity/unity-engine-landscape-swimlane.png?v=qXuAEuTmn1teWmBipAskcg5IpW6Tn2fEunOIqAYui20)
<h1 align="center">Hi there 👋 I' m Ender Erol</h1>
<h3 align="center">I'm passionate Software Engineer, Swimming Coach and interested with XR.</h3>

- 🔭 I’m currently working on **ReoTek as a Unity Developer.**

- 🌱 I’m currently learning **C#, Python, Unity, OpenCV**

- 📫 How to reach me **endererol.work@gmail.com**

- https://leetcode.com/roxender/ for individual practice

<h3 align="left">Connect with me:</h3>
<p align="left">
<a href="https://linkedin.com/in/endererol-gd" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="endererol-gd" height="30" width="40" /></a>
<a href="https://www.youtube.com/c/endererol9554" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/youtube.svg" alt="endererol9554" height="30" width="40" /></a>
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://www.w3schools.com/cs/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/csharp/csharp-original.svg" alt="csharp" width="40" height="40"/> </a> <a href="https://www.figma.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/figma/figma-icon.svg" alt="figma" width="40" height="40"/> </a> <a href="https://git-scm.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/> </a> <a href="https://opencv.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/opencv/opencv-icon.svg" alt="opencv" width="40" height="40"/> </a> <a href="https://postman.com" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/getpostman/getpostman-icon.svg" alt="postman" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://unity.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/unity3d/unity3d-icon.svg" alt="unity" width="40" height="40"/> </a> </p>


<p>&nbsp;<img align="center" src="https://github-readme-stats.vercel.app/api?username=endererolwork&show_icons=true&locale=en" alt="endererolwork" /></p>

<p><img align="center" src="https://github-readme-streak-stats.herokuapp.com/?user=endererolwork&" alt="endererolwork" /></p>


__________________________________________________________ PROJECTS _________________________________________________________________________
The video and code snippets I have shared below have been used to promote the projects I have developed within Reo-tek.

LİDAR Bacterial Defence Game Project

In the Phytopathogens Digital Table project, an application was developed using photographs of numerous bacteria. These photographs depict the bacteria as if they were floating within cells, and they also include detailed information about each bacterium.

UDP data coming from Lidar was taken and processed and integrated into the project as windows mouse touch.
```ruby
using System.Net;
using System.Net.Sockets;
using System.Text;
using UnityEngine;

public class LidarController : MonoBehaviour
{
    public int port = 3333;
    private UdpClient udpClient;
    private IPEndPoint remoteEndPoint;
    private Baloon balloon;

    private void Start()
    {
        udpClient = new UdpClient(port);
        IPEndPoint remoteEndPoint = new IPEndPoint(IPAddress.Parse("127.0.0.1"), port);
        balloon = FindObjectOfType<Baloon>();
    }

    private void Update()
    {
        if (udpClient.Available > 0)
        {
            byte[] data = udpClient.Receive(ref remoteEndPoint);
            string lidarData = Encoding.ASCII.GetString(data);

            // Use lidarData to trigger mouse down event in Baloon script
            if (lidarData == "trigger")
            {
                Debug.Log("Lidar data received: " + lidarData);
            }
        } 
    }

    private void OnDestroy()
    {
        udpClient.Close();
    }
}
```

https://github.com/endererolwork/endererolwork/assets/112380859/92cd4fb9-175b-4fda-b360-c1ab29b0ec28

Book Reviewing Game with Camera Project

https://github.com/endererolwork/endererolwork/assets/112380859/d469ea82-c25f-4b6b-a6fe-e8cd30823d00

DNA Project

https://github.com/endererolwork/endererolwork/assets/112380859/de8c35ec-0e46-4d69-97e4-54a5a0b3e818

Species Pool Project

https://github.com/endererolwork/endererolwork/assets/112380859/29126d8c-7b66-45b3-ba8a-d7091484f203

Phytopathogens Digital Table Project

https://github.com/endererolwork/endererolwork/assets/112380859/908e157c-e13e-44ed-8276-48f942cb16d4

Biological Defence Project

https://github.com/endererolwork/endererolwork/assets/112380859/507f828f-2877-4208-8019-19808acddcb3


Tubitak Health and Safety Executive VR Project

https://github.com/endererolwork/endererolwork/assets/112380859/f27a5644-53aa-4a0e-ad58-63ea1646a117


https://github.com/endererolwork/endererolwork/assets/112380859/08f6a5c6-5910-433a-ab72-93bbd862ce7b


