## Mission Overview 
Congratulations,  
Your onboarding has been successfully completed, and your Cloud Computing Portfolio has been approved by your supervisor.CloudNova Technologies has now assigned you to your first official project. Before deploying cloud services, every cloud engineer must understand the infrastructure that powers modern cloud computing. Your mission is to investigate the components of cloud infrastructure, identify how compute, storage, networking, and identity services work together, and document your findings as if you were preparing technical documentation for a client. Using the KillerCoda Playground, Linux tools, official cloud documentation, and your GitHub Cloud Computing Portfolio, you will complete a series of engineering tasks that simulate the planning phase of a cloud deployment. 

## Mission Objectives 
At the end of this laboratory activity, you should be able to: 
- Explain the major components of cloud infrastructure.  
- Investigate the hardware and software resources available in a Linux environment.  
- Differentiate compute, storage, networking, and identity resources.  
- Interpret the relationship between cloud infrastructure components.  
- Create professional technical documentation using Markdown.  
- Continue building a structured GitHub Cloud Computing Portfolio.

## Cloud Infrastructure Components

| Component            | What I Found                                          |
| -------------------- | ----------------------------------------------------- |
| Compute Resources    | Intel Xeon E312xx CPU with 1 CPU core and 1.9 GiB RAM |
| Storage Resources    | 19G disk capacity with mounted file systems           |
| Networking Resources | IP addresses `172.30.1.2` and `172.17.0.1`            |
| Operating System     | Ubuntu 24.04.4 LTS                                    |

## Tools Used

| Tool                   | Purpose                                                          |
| ---------------------- | ---------------------------------------------------------------- |
| KillerCoda Playground  | Used to access the Linux server and perform the laboratory tasks |
| Linux Terminal         | Used to run commands and collect system information              |
| GitHub                 | Used to store and organize the laboratory documentation          |
| Markdown               | Used to format the README file                                   |
| Web Browser            | Used to access KillerCoda, GitHub, and other references          |
| Draw.io (diagrams.net) | Used to create the cloud infrastructure diagram                  |

## Linux Commands Executed

| Command                      |
| ---------------------------- |
| `cat /etc/os-release`        |
| `uname -r`                   | 
| `lscpu \| grep "Model name"` |
| `nproc`                      | 
| `free -h`                    |
| `df -h`                      |
| `findmnt`                    | 
| `hostname -I`                |

## Skills Learned

I learned how to use basic Linux commands to investigate the resources of a server. I was able to collect information about the CPU, memory, disk, operating system, mounted file systems, hostname, and IP addresses.

I also learned how to organize the collected data into different cloud infrastructure components. The activity improved my skills in using the Linux terminal, writing Markdown documentation, and managing laboratory files through GitHub.

## Challenges Encountered

| Challenge                           | How I Handled It                                                                                      |
| ----------------------------------- | ----------------------------------------------------------------------------------------------------- |
| Reading the output of `findmnt`     | I reviewed the listed file systems and checked which ones were mounted.                               |
| Finding the IP address              | I used `hostname -I` to correctly display the available IP addresses.                                 |
| Identifying the different resources | I categorized the information into compute, storage, networking, and operating system resources.      |
| Organizing the README               | I used Markdown tables, headings, and backticks to make the documentation clearer and easier to read. |


