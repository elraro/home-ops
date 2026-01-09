<div align="center">

<img src="https://github.com/elraro/home-ops/assets/1223299/6b9ff5ed-5272-4122-afee-81073ed84de0" align="center" width="144px" height="144px"/>

### My home operations repository :octocat:

_... managed with Flux, Renovate and GitHub Actions_ 🤖

</div>

# Requirements

```
# install pre-commit
pip install pre-commit --break-system-packages
echo 'export PATH=/home/$USER/.local/bin:$PATH' >> ~/.bashrc

# install sops
curl -LO https://github.com/getsops/sops/releases/download/v3.8.1/sops-v3.8.1.linux.amd64
mv sops-v3.8.1.linux.amd64 /usr/local/bin/sops
chmod +x /usr/local/bin/sops

# install direnv
apt install direnv
echo 'eval "$(direnv hook bash)"' >> ~/.bashrc

# install fluxcd
curl -s https://fluxcd.io/install.sh | sudo bash
echo '. <(flux completion bash)' >> ~/.bashrc

# configure GITHUB_TOKEN and GITHUB_USER
echo 'export GITHUB_TOKEN=<your-token>' >> ~/.bashrc
echo 'export GITHUB_USER=<your-username>' >> ~/.bashrc
```
