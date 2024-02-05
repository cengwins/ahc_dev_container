# Building and Running

1. Install docker, vscode and docker extension in vscode
2. Clone this repo `https://github.com/cengwins/ahc_dev_container.git`
3. Open ahc_dev_container folder in vscode, open a terminal and build docker image `docker build . -t ahc_dev_container`
4. On docker extension of vscode, run ahc_dev_container image in interactive mode
5. In terminal run `docker run -t -i --rm --privileged --cap-add=NET_ADMIN --name ahcdev -v ./code:/root/code:rw ahc_dev_container:latest bash` and keep this terminal running.
6. Create a public project on GitHub by cloning https://github.com/cengwins/ahc_distalg_template.git
7. In the container: clone your project in to `/root/code`, this directory is a RW directory mapped to your `code` directory on your host!
