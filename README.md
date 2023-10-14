# nanoGPT
My experience in getting nanoGPT to work in LinuxMint
Here are some things which, after going through this, I wish I knew BEFORE getting started.
1) You can waste a lot of internet bandwidth doing this multiple times. I would love to know how to download files that PIP installs locally and instruct PIP to pull from there.
   - this is listed first because I do not have UNLIMITED bandwidth. I have never exceeded the 1.25TB limit my provider has in the well over 10 years of being with them.
   - however, I might this month. In one day, my usage was 170GB (about 60 of it was from my kid downloading a game/updates) 
   - some of the big files were: The CUDA library installed by pytorch(2.5GB), gpt2-xl model(+4GB), other libraries, anaconda, etc, linux updates ( Ubuntu bombed hard for me, used to be solid, now is not so much)
2) How to plan the installation in Linux.
   - maybe you want anaconda available to all users and it should be installed somewhere specifically? /opt, for example.
   - should you consider having more than one user in linux for developing? If so, put in same group, update certain global profile settings, etc.
3) Once sample project is runnable, how does one get "creative?"
     - The sample was "infinite shakespear", so naturally, I wanted to try an "infinite Twain"
     - How does one actually finetune a model? ( sample provided a script that was to use gpt2-xl, which author explained would take like 4 days on an A100 node ( that's 8xA100 with 40GB)\
     - My car isn't even worth one A100, let alone 8. I checked and at it would cost about $1700.00 to use cloud resources.
     - FYI - Will not run on 3060TI with 12GB. Had to swap to medium model.
       
