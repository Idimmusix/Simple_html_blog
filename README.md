To deploy on the server.
1. Spin up a GCP VM instance - ubuntu 22.04
2. ssh into the instance
3. update the apt repository using `sudo apt update`
4. Upgrade the packages in the ubuntu machine
5. install nginx using `sudo apt install nginx`
6. clone the repo on `/var/www` using `sudo git clone https://url-to-repository.git`
7. cd into the repo and change the owner using `sudo chown -R $USER: .`

8. In github UI, setup self-hosted runner on the VM instance by going to github >> settings >> actions >> runners
9. In your local VS code, create your deployment file for your code in the `.github/workflows` directory.
10. Push to github and ensure that it runs successfully in the ations tab.