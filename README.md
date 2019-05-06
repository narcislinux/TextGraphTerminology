## Text Graph Terminology

### Uniform Resource Identifier (URI)


          userinfo     host        port
          ┌─┴────┐ ┌────┴────────┐ ┌┴┐
          https://user@www.example.com:123/forum/questions/?tag=networking&order=newest#top
          └─┬─┘ └───────┬────────────────────┘└─┬─────────────┘└──┬───────────────────────┘└┬─┘
          scheme     authority                 path              query                 fragment


### libvirt Terminology and goals

		 ________________
		|  ________      |      ___________________________________
		| |_Domain_| Node----> |A node is a single physical machine|
		| |_Domain_|     |      ____________________________________________________________
		| |_Domain_|-----|---> |a domain is an instance of an operating system (or subsystem|
		| |_Domain_|     |     |in the case of container virtualization) running on a       |
		| |_Domain_|     |     |virtualized machine provided by the hypervisor._____________|
		|  ____________  |      ___________________________________________________________
		| |_Hypervisor_|-|---> |an hypervisor is a layer of software allowing to virtualize|
		|________________|     |a node in a set of virtual machines with possibly different|
                                   | configurations than the node itself.______________________|