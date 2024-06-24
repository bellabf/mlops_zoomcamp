# Mage
Mage is a general purpose tool to do workflow orchestration.

## Setting up mage instructions

I did this on codespaces since I'have been having fun using it :) 

1) Clone repo at https://github.com/mage-ai/mlops.git
2) The docker compose file has a line " ~/.gitconfig:/root/.gitconfig:ro" that requires us to have a gitconfig file, but there is no such file in codespaces. If you just execute it, next time it will complain (because it is not file, it is a folder). You should create the gitconfig in the home of your codespace. Once that is done you can proceed as usual.
3) All is good to go! Follow mage tutorial