
<img src="https://user-images.githubusercontent.com/31302079/153671583-4214e7d0-2a3e-4478-83c1-4c1f62d0f87c.png" alt="drawing" width="100%"/>

# Best Users Network-Ending Treaty
#### A prototocol based on Dijkstra algorythm to syncronize hosts lists for peer-to-peer netwok. Supplementary project for Networks Coursework, made up quick-and-dirtyin a garage in couple hours, but I'm satisfied a lot 
#### You are able to use it in command line and as a module in Python as well and pass command arguments to `bunet` program

Ready for usage on multiple machines, but tested on single with many users. Requests are performed via ssh: `ssh username@hostname command`. But it is adviced to create user `bunet` and create `~/.config/bunet` in his home directory

### Usage:
```
usage: bunet [-h] {get,save,buildnet,buildnet-share,share,add,clear} ...

options:
  -h, --help            show this help message and exit

command:
  Action to perform

  {get,save,buildnet,buildnet-share,share,add,clear}
                        Command description
    get                 Get node's hosts list
    save                Add your entered hosts to node's list
    buildnet            Retrieve all hosts from network
    buildnet-share      Retrieve all hosts from network and share this list with others
    share               Share your existing hosts list with others
    add                 Add new nodes via arguments
    clear               Remove bunet list
```

### Requirments
- `python3`
- `ssh` and exchanged SSH keys for password-less authentication of only your node with others
- `bunet` is placed in `/usr/bin` or used anyhow else to act like bash-y command
- User(node) is owner of `~/.config`

Hosts list is stored in `~/.config/bunet`
