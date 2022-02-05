
<img src="https://user-images.githubusercontent.com/31302079/152659751-3ca436d7-cbde-41e7-abcc-79026b1b6266.png" alt="drawing" width="100%"/>

# Best OOsers Broadcasting Interlinking-Ending Statut
#### A prototocol based on Dijkstra algorythm to syncronize hosts lists for peer-to-peer netwok. Supplementary project for Networks Coursework, made up quick-and-dirtyin a garage in couple hours, but I'm satisfied a lot 

Works fine for single machine and multiple existing users. Takes just few changes to work on multiple real hosts. Maybe, I'll change it later to work on many machines

### Usage:
```
$ boobies [command]

Possible commands are:
	get - to retrieve list of known nodes
	save - to suggest saving of my list
	share - to share your list with other nodes
	buildnet - recursive get, i.e. asking all new nodes
	buildnet-save - recursive get and sharing with all nodes we know
```

### Requirments
- `python3`
- `ssh` and exchanged SSH keys for password-less authentication of only your node with others
- `boobies` is placed in `/usr/bin` or used anyhow else to act like bash-y command

Hosts list is stored in `~/.config/boobies`
