
curl -L "https://packages.gitlab.com/install/repositories/runner/gitlab-runner/script.deb.sh" | sudo bash

sudo apt-get install gitlab-runner

apt-cache madison gitlab-runner

To register a runner under Linux:

sudo gitlab-runner register

https://gitlab.com/

GR1348941cHffwsEJ3ugyth5cuD54

shell

sudo gitlab-runner -version
