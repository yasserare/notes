   # notes
My Notes about anything especially programming / tech related.


# Virtualization
- It essentialy means creating a simulation of hardware or software in a software environement.
- Its uses:
    * Running multiple Operating systems and computers from the same computer and operating system.
    * 
# Superintelligence  
- Ways of reaching AGI:  
   * AI:  
      - core Features (These are Features that should be considered while developping and are not an after thought):  
            * It should be able to learn.  
            * dealing with probablity and uncertainty.  
            * derive concpets from sensory data and use them (concepts) in reasoning.  
      - Everything evolution acheieved, Human engineering can achieve tha same.including AI (opposed to human intelligence) as moravec said:  
      `The existence of several examples of intelligence designed under these
      constraints should give us great confidence that we can achieve the same in
      short order. The situation is analogous to the history of heavier than air flight,
      where birds, bats and insects clearly demonstrated the possibility before our
      culture mastered it`  
      - computation power is the issue here, we need super computers to run algorithms so we can mimic >= human level intelligence.  
      - even with moore's law, It will probably take so long to reach computation that would help reach AI.  
   * Whole brain emulation:
      - Taking a dead person's brain, slicing it, scanning it and producing a software version of the brain that can either inhabit a robot or just be ran virtually on a pc.
      - It does not need any Major breakthroughs but it needs very advanced technology.
      - The technological capabilities needed to reach whole brain emulation are much more then AI.
      - ALthough not entirely, This path is less dangerous than the AI path because we can see it coming from a mile way (not entirely) because it will needs to work on multiple organisms before it works on humans. (see Whole brain emulation roadmap)
   * biological cognition:
     - Actaully "Improving" the human brain through techniques such as iterative embryo selection and other techniques.
     - It will probably take too much to achieve superintelligence whereas Previous techniques like AI might have already reached superintelligence.
   * brain-computer interfaces:
     - Basically means cyborgs, Imagine something like DBS system for parkinson but way more advanced.
     - but this path is unlikely because such system could cause so many complications and other paths are way more feasible and have lower risks for the safety of the user.
   * Networks and organizations:
      - Imagine a web or organization where only highly intelligent people connect with each other, share informations and their only objective individualy is to engage in highly intelectual disscusions.
# AGING  
# SSH  
   * Secure Shell (which is not a shell at all, the name comes from the rsh program which is used for remote login) is a program that enables logging into a remote machine and excuting commands on that machine, it is also be used in other tools such as  sftp and scp to transfer files (s in sftp and scp stands secure and they are upgrades of ftp and rcp which are the original versions).  
   * it core benefit is its security, thus replacing programs like telnet and rlogin which are both used for remote login and rhs for remote login.  
   * ssh is not a shel in the same sense of a bash, it does interpret commands or have commands history or anything like that.  
   `[questions to answer] `  
      `how does it really work ? like really ?`  
      `how do sys admins actually use it ? and how normal users can use it ?`  
       `read that summary`
# apt vs aptitude:  
   * both package managers in linux systems.

# Deep Work  
   - at the 27th, farm log time asap and then disappear deep work for the rest of the month.  
   - Ritualize:  
        * Find a super peaceful place and work inside it for a long time and make it a habit.  
        * Make boundaries, what you can and can't do during a deep work session some people might find it better to not use the internet at all or maintain a metric.  
             - No phone Usage at all, No youtube[except for learning, maybe use an extension that hides youtube conten], No Discord, no entertainment, No Music, break outside the work place, avoid small talks, have a place where you only do deep work thus you automatically expect of yourself to focus intensely whenever you are in that environment.   
             - maybe think of a metrics (like reaching a predefined goal that you find appropiate).     
        *  Create support, preparing and tweaking your body to work more deep:
             - for some people it might be a good cup of coffee, for others it might be a good exercise.
             - for me, I should not be hungry or unhydrated, tired (Sleep) or thinking (Meditation) about anything too much conciousely and unconciousely.  
        * Make a grand gesture:
             - Make huge efforts to provide a deep work session, the bigger the effort the better. This will conciousely and unconciousely will stress you (in a good way) to go deeper than usual.
        * Open offices and 13 like places are great places for miracles to happen especially when there is diversity in disciplines, but it open working places should be combines with sound proof closed rooms(not necessarily this exact idea, it could be just your own home desk) for deep work.
         
# LVM (Logical Volume Management):  
   * IT is a form of Storage virtualization.  
   * It means making a pool of storage out of multilple storage devices, creating at least one logical volume and manipulating it with much more flexibility as needed. in noob terms, it means taking multiple storage devices and making them seem like one huge chunk of storage, Modifying that chunk(logical volume) as needed(creating new logical volumes, resizing them).  
   * Main terms:
        - Volume Groupe: The physical pool of storage devices.  
        - Logical Volumes: The partitions that are created in that volume Group.  
   * It general Uses:
      -  The ability to virtualze storage.  
      -  For a better backup: you can create a snapshot volume that is an exact copy of the volume you need to backup, it saves in that exact moment you made that snapshot volume, you can do this while still working in that same original volume.
      -  Resizing: unlike gparted for example, you can resize a partition regardless of its surrounding partitions state, meaning that you don't need a a logical volume to be contiguous with another free space to resize the logical volume.
      -  you can do most operations without the need to run from a live OS, meaning you can do these operations without the need to reboot, umount or format anything.
      -  (to be tested) You can LVM  your dual boot for much better use of storage.  
   * sys admins Uses:  
     - Increase A web server's storage without the need to take offline. (using classic partitions would push the sys admin to unmout and take the website offline).  
     - Backup server data withsnapshots without the need to reboot or take the server offline.  †
 # SUDO:
    * Installed by "su root" then "apt install sudo".  
 # UFW:  
    * What is a firewall ?  
         - It is A software or device (usually a software), that monitors and filter network traffic thus providing a level of protection to the user.  
    * UFW: It's a frontend program for the tool iptables which is an interface for using netfilter.  
          - Netfilter is kernel-level program that actually does the packet filitering  and packet mangling.
    * Packet: the actual Data and additional importan informations  
         - Example: you visit a website => packet get sent to the server with your IP and the server's IP => server firewall accepts => server send you back the packet with the HTML code, ITs IP address and your IP address  and the source and destination ports in the header.  
    * Packet filtering: Is the firewall's ability to accept or deny the passing of a packet based on predefined rules.  
    * Packet mangling:  
    * IP address: 
    * Ports: 
     
