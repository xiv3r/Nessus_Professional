# <h1 align="center">Nessus Professional</h1>

<p align="center">Nessus Professional stands as a powerful and versatile vulnerability assessment solution, empowering organizations of all sizes to fortify their cybersecurity posture. Its comprehensive vulnerability coverage, rapid asset discovery, configuration auditing, target profiling, malware detection, and sensitive data discovery capabilities make it an invaluable tool for mitigating cyber threats. </p>
<br></br>

### Setup

    docker pull ramisec/nessus
    
    docker run -d --name=nessus -p 8834:8834 ramisec/nessus
    
    docker exec -it nessus /bin/bash /nessus/update.sh


### Updating the Plugins

    docker exec -it nessus /bin/bash /nessus/update.sh


### Username & Password

Username: `admin`

Resetting the Password by running 

    docker exec -it nessus /opt/nessus/sbin/nessuscli chpasswd



Example output:
```
Login to change: admin 

New password: Password123!

New password (again): Password123!

Password changed for admin

```

## Now open [Google Chrome](https://localhost:8834)
