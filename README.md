# SchedulerChatBot

## Environment Setup

### Create a Google Cloud VM Instance

1. Create new project called scheduler chat bot
2. Open project
3. Pin Compute Engine from sidebar (optional)
4. Compute Engine > VM Instances > Create
5. Change machine type to e2-standard-8 (8 vCPU, 32 GB Memory)
6. Change Boot Disk to 
  - Operating system: Debian
  - Version: Debian GNU/Linux 10 (buster)
  - Size: 100 GB
7. Allow HTTPS Traffic
8. Create

### Connect to and setup a Google Cloud VM Instance

1. Connect > Dropdown > View gcloud command (Copy this)
2. `gcloud auth login` in a new terminal
3. Run gcloud ssh command; should look like this `gcloud beta compute ssh --zone "us-central1-a" "instance-1" --project "schedulerchatbot-303906"`
4. `python3 --version` is 3.7.3
5. Update package list: `sudo apt update`
6. Install git: `sudo apt install git`
7. Install pip3: `sudo apt install python3-pip`
8. Upgrade pip3: `pip3 install -U pip`
9. `pip3 --version` should be 21.0.1
10. Install rasa: `pip3 install rasa`
