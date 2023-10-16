# <h1 align="center">Nessus Professional</h1>

<p align="center">Nessus Professional stands as a powerful and versatile vulnerability assessment solution, empowering organizations of all sizes to fortify their cybersecurity posture. Its comprehensive vulnerability coverage, rapid asset discovery, configuration auditing, target profiling, malware detection, and sensitive data discovery capabilities make it an invaluable tool for mitigating cyber threats. </p>
<br></br>



### Requirements

     sudo apt install docker.io


### Setup

    git clone https://github.com/xiv3r/Nessus_Professional.git

    wget https://github.com/xiv3r/Nessus_Professional/releases/download/Nessus/backup-image-ramisec_nessus.tar.gz
    
    sudo docker pull ramisec/nessus
    
    sudo docker run -d --name=nessus -p 8834:8834 ramisec/nessus
    
    sudo docker exec -it nessus /bin/bash /nessus/update.sh


### Updating the Plugins

    sudo docker exec -it nessus /bin/bash /nessus/update.sh


### Username & Password

Resetting the Password by running 

    sudo docker exec -it nessus /opt/nessus/sbin/nessuscli chpasswd


Add New User and Password:

Login to change: `admin`

New password: `Password123!`

New password (again): `Password123!`


## Now open [Google Chrome](https://localhost:8834)
