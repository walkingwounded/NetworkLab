* Installing Trend Micro Agent on a Headless Server (Lenovo ST50 - Windows Server 2019) *
Date: 15-May-2025
Objective: Successfully install the Trend Micro Agent on a Lenovo ThinkSystem ST50 running Windows Server 2019 Standard.

✅ Summary:
Today, I overcame a real-world IT challenge that tested both my practical knowledge and my resourcefulness. I successfully installed the Trend Micro Agent on a headless server (i.e., no monitor attached), with minimal information provided—only the server hostname and administrator credentials.

🧱 Challenge:
The Lenovo ST50 server had no monitor connected and no IP address was provided.

The previous IT vendor was uncooperative, and left behind no documentation.

I had no physical access, and had to work with just:

Server name (hostname)

Admin username and password

🧠 Solution:
I recalled what I learned from the TryHackMe RDP Lab, particularly how Remote Desktop Protocol (RDP) can be used effectively in low-visibility situations.

Steps I Took:
Used mstsc (Remote Desktop Client) with the server name:

bash
Copy
Edit
mstsc /v:[server-name]
Pro Tip: If DNS is properly configured in the environment, a hostname can resolve without needing an IP address.

Successfully established an RDP session using just the hostname and credentials.

Verified the system environment, ensured compatibility, and performed the installation of Trend Micro Agent without any graphical hiccups or direct interaction.

Tested and confirmed that the agent was installed and communicating with the central console.

💡 What I Learned:
Even with limited access and information, it's possible to navigate and resolve IT tasks using basic but powerful tools like mstsc.

DNS resolution and Active Directory integration can often save the day in corporate networks.

My hands-on learning from TryHackMe labs is not just academic—it's genuinely applicable to live environments.

📝 Reflection:
This was more than just a software installation. It reinforced the value of self-guided learning, problem-solving under constraints, and the confidence to handle enterprise-level infrastructure issues. I'm proud of how I managed this task independently.

