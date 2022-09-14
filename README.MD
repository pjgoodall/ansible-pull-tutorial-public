# ansible-pull-tutorial-public

Nothing much to see here - following along 
[Using Ansible "Pull" Mode to Dynamically Automate Server/Workstation Builds](https://www.youtube.com/watch?v=sn1HQq_GFNE&t=3s&ab_channel=LearnLinuxTV) 

The challenge will to be to replicate this process wth a private repository. ansible-pull from within a private repository seems to generate a lot of opinion, but very few examples.

## Journal

1. made a branch `zero` for basic operation - KISS
2. had problems with -- include of task - so made it into one file
3. Needed to prefix the `ansible-pull` with `sudo` because of the `become: true`

```
sudo ansible-pull \
    -U https://github.com/pjgoodall/ansible-pull-tutorial-public.git \
    -C origin/zero

```
