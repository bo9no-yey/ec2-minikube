# ec2-minikube

1. Run setup.sh

    ```bash
    ./setup.sh
    ```

2. Add a user for remote desktop and restart

    ```bash
    sudo adduser [username]
    sudo gpasswd -a [username] sudo
    sudo reboot
    ```

3. Run minikube start as root user

    ```bash
    minikube start --vm-driver=none
    minikube addons enable ingress
    ```

After implementation, remote desktop is possible with ec2-host name.