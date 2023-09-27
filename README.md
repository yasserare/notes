   # notes
My Notes about anything especially programming / tech related.


# Virtualization
- It essentialy means creating a simulation of hardware or software in a software environement.
- Its uses:
    * Running multiple Operating systems and computers from the same computer and operating system.
#Evaluation
	- Be polite, stimulate a coding review at work with a co worker.
	- It should be at least 15 to 20 minutes.
   	- Check norm first, no unimportant norm error.
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
# AppArmor  
   * Kernel Module Security application for linux, it's used to sandboxe process and give the minimum previlege needed.
   * to check if it is enabled `aa-status`.
   * It is used to confine process from accesing files they should not have access to.
   * example: A server hosting multiple websites, confine each website and give it least previlege needed to prevent it from accessing other ressources even if it is compromised.
   * A website in /home/user/Documents/website-name/ shoulde not have access to files in /home/user/Documents/website_number_two/ or why give it access to system calls or the camera when it does not need them.
   * it difference with SELinux: 
   ? Does it prevent website process (in the example of a server hosting mutiple websites) from accessing other ressources [try it maybe].
# lsblk  
	* tool to list block devices (storage devices).  
# disk Signature  
   * A long hexadecimal which is the ID of the virtual disk.  
   * It is a security mechanisme to prevent the alteration of the virtua disk.  
   * It is created using the shasum command (see the subject for more informations).  
   ? LOOK INTO HOW DOES SHASUM PREVENT SIGNATURE DUPLICATION.
# debian vs rocky  
	* I chose debian because i am familiar with installing debian based os's, and also because the subject claim that it is easier to install debian than rocky.  
 	? maybe just maybe try to install rocky os.  
# SSH  
   * Secure Shell (which is not a shell at all, the name comes from the rsh program which is used for remote login) is a program that enables logging into a remote machine and excuting commands on that machine, it is also be used in other tools such as  sftp and scp to transfer files (s in sftp and scp stands secure and they are upgrades of ftp and rcp which are the original versions).  
   * it core benefit is its security, thus replacing programs like telnet and rlogin which are both used for remote login and rhs for remote login.  
   * ssh is not a shel in the same sense of a bash, it does interpret commands or have commands history or anything like that.  
   `[questions to answer] `  
      `how does it really work ? like really ?`  
      `how do sys admins actually use it ? and how normal users can use it ?`  
       `read that summary`
  * Install ssh => sudo apt install openssh-server  
  * port 22 is the defult for ssh (use `sudo systemctl status ssh`).
  * to change the port, edit the file `/etc/ssh/sshd_config` and restart the service using `sudo systemctl restart ssh`
  * ip a - To check the IP to use for connect from the host terminal.
    	ssh <vmusername>@<vmip> -p 4242 - (In the host terminal) to connect to the VM using ssh.
# apt vs aptitude:  
   * both package managers in linux systems.
# Computer architecure:  
   * 
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
    * configuration:
    	- The configuration is done in visudo.  
     	- Defaults requiretty
     	- Defaults passwd_tries=3 - To set the number of password attempts when using sudo to 3.  
	- Defaults badpass_message="Wrong password" - The error message due to a wrong password.  
	- Defaults logfile="/var/log/sudo/sudo.log" - To create and set the log file.  
	- Defaults log_input,log_output - To create the logs of the inputs and outputs of every use of sudo.  
	- Defaults iolog_dir="/var/log/sudo" - The directory where those logs will be stored (created previously).  
	- Defaults secure_path="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin" - To restrict the PATHs that can be used by sudo specifically to those specified.  
 	- TTY:  TTY is the Operating system's way of differentiating between ssh remote login and local shell user or between multiple remote users.
  		Example: a Programmer open a sudo session using ssh and start working on a website that has a database, 
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
    	- write meaning here  
      	- install ufw using apt, enable it using `sudo ufw enable`, allow a specific port using `sudo ufw allow 4242/tcp or (4242/udp)`   
        - sudo ufw status is also a useful cool command.  
# hostname:  
    * Research its purpose.  
    * use `hostname` to display the current hostname.  
    * use `sudo hostname new-hostname`  to temporarily change the current sessions hostname.  
    * to change the hostname forever, edit the files: `/etc/hostname` and `/etc/hosts`.  
    * sudo hostnamectl set-hostname <newhostname> - Changes the hostname.
    	   sudo nano /etc/hosts - And then change the old hostname for the new one
# groups and users:  
    * Create a new group: sudo groupadd nameofthegroup.  
    * Add users to a group, sudo usermod -aG groupsname user.  	
    * Create a user: sudo adduser nameofthenewuser.  
    * Get users of a group.  
# cron script:
	* Wall: simply a command to that enables you to show a message to all users.  
 	* To stop a cronta: run `crontab -e` => delete the crontab command => save.
  	* Infos:
   		1 uname -a  
     		2 lscpu
       		3 free -h (-h for human readable format)
	 	4 
   		5 
     		6 
       		7 who -b
	 	8 
   		9 who
     		10 
       		11 sudo cat /var/log/sudo/sudo.log | grep COMMAND | wc -l (test it with minimal number of commands)  
# Strong password policy  
	* Install libpam-pwquality (to be researched).  
	* First three rules, edit variables `PASS_MAX_DAYS`, `PASS_MIN_DAYS` and `PASS_WARN_DAYS` in the file /etc/login.defs.    
 	* Edit the file  /etc/pam.d/common-password in the line under [ #here are the per-package modules (the "Primary" block)]: 
  		`
		minlen=10 - Sets the minimum acceptable size for the new password to 10.
    		ucredit=-1 - The password must contain an uppercase letter.
      		lcredit=-1 - The password must contain an lowercase letter.
    		dcredit=-1 - The password must contain a digit.
    		maxrepeat=3 - The password must contain more than 3 consecutive identical characters.
    		reject_username - The password must not include the name of the user.
    		difok=7 - The password must have at least 7 characters that are not part of the former password (does not apply to the root password).
    		enforce_for_root - The root password has to comply with this policy.
		`
  	* sudo chage -M 30 <user> and sudo chage -m 2 <user> expiary dates for both user.  
  	
[git and github]

	-restore a file from the last commit
		git checkout <commit> <file>
	-list last commit
		git log
	-list branches
		git branch
	-switch branches 
		git checkout <nameofbranch>
	-delete beanch
		git branch -d <nameofbranch>
	-create a new branch
		git checkout -b <nameofnewbranch>
	-Making a pull request
		git add <FILES>
		git commit -m "messgae"
		git push origin <nameofbranch>
		=> go to the original repository and create pull request
	-reset to the original repo
		git reset --hard origin/master
	-contribute to repo that you deleted locally
		re clone
		git branch -a
		git checkout <branchname>
		make changes	
  	-display git commits history / see divergent branches
		git log --graph --oneline --all

[grep]
	-Search for a word or sentce in the current directories and sub directories
		grep -r "testKeyword" .	

[Keyboard shortcuts and cli commands]
	-Move current application to another workspace
		shift + ctrl + alt + arrow 
	-Count how many lines ls will dispay
		ls | wc -l 
  	-Vscode multiline comment
   		ctrl + atl + a
[algorithms]
-steps tp accomplish a task
	algorithm of solving coding problems:
		-deeply understan the issue
		-you will get a solution in mind, trying to come up with an aditional one 
		-divide the solution into small parts
		-implement the solution part by part

[scanf]
be wary of the following:
	scanf("%c", &c) is not the same as scanf(" %c", &c) => the latter ignores any white spaces when reading input while the former does not.

[make and makefile]
make = automation tool 	=> generate executables and non-source files from source files
makefile = file  => run tools according to the instructions in makefile 

Make looks for makefile ( make file has instructions on how to generate the non-source files(example: executable, static library)).

why do we need make ? we could just use the compiler directly.
you could use the compiler directly but it is to much work(you'd need to specify each file you want to compile and there could be hundereds of source code files)
make also has the advantage of running multiple different commands with 1 simple command 
(instead of compiling to object files and then creating a static library => you could just run make and that's it)
 syntax:
- make RULES
	target: dep
		command
*a rule is an instruction in makefile for make
	target  = the target file we want to generate
	dep	= are files that the target files need to have in order to exist
	command = the command in which we will use dep to generate target 
*you can specify which rule Make should start with but by default, it goes to the first rule.
*when you run Make, it does not update all target files each time you run it, it instead compares target file with all of it dep, if it is newer than all of them,
	it does nothing(target file being newer than all of its dep means that target file was the last created file in comparaison to its source files)

================================================================
[malloc] = allocate memory inside the heap in bytes
	malloc asks OS 1 byte =>  OS searches the heap for it => if found => that byte marked as used => pointer to beginning of the block is returned
								=> not found => do memory management operations => not found => return NULL
	the allocated memory is not initialized with anything, if you want it to be initiliazed use calloc.
[OS]
1 transistor = 1 bit
	16 gb of ram = 128000000000 bits = 128000000000 transistors
the binary for the digit 1 = 00000001 = 7 off transistors and 1 on
=== the key press pipeline ===
Atoms = The smallest thing in the universe, everything in the universe  consists of atoms
	Its syntax (hh) ATOM = nucleus(protons + neutrons) + electrons( orbiting around the nucleus).
[bootloaders]
the first program a PC runs when started or restared. It tests the hardware (check if each hardware component(CPU, RAM, strage device ....) is working properly)for the OS

[libft]
A variable is a storage area in memory nad has the following characterestics:
	1. name
	2. data type
	3. value
	4. Scope (global vs local)
	5. lifetime (throughout the whole program lifetime or a function's lifetime)
dynamicaly allocated memory (such as with malloc) is stored in the heap.
Integer Overflow is when we assign a variable a value that bigger than the biggest value it can represent 
Integer Underflow is when we assign a variable a value that smaller than the value that it can represent

size_t (unsigned int) => it's not overflow, it's wrapping back to 0 (https://wiki.sei.cmu.edu/confluence/display/c/INT30-C.+Ensure+that+unsigned+integer+operations+do+not+wrap)
	size_t x = SIZE_MAX; x + 1 => printing x would print 0
size_t == unsigned integer 
size_t x = 0; x - 1 would wrap. 

Memory leaks
	
[strlcat]
	the reason for the if statemnent is because if size == 0 then (size - 1 == huge positive number)
what is a static library ? it is the collection of the object files. its purpose is to cut down time and effort for programmers and make it easier to code.
what is Locale in isalpha ? a "locale" the a set of cultural settings(language for example)
	example: if current user's locale is set to greek, isalpha would consider the character 'β' a alphabetical character since it is a greek character
			but it won't consider it a alphabetical character if the locale is set to english because it is not a english alphabet.
why main has type int and returns 0 ?
	by convention, 0 implies to the OS that the program ran succesfully, if a non-zero value is returned, it indicates to the OS that the program did not run
		correctly. that information (that a program ran correctly or not) is useful for the user so they know that the program did not work as intended
			(the programmer can show an error based on that return value of non-zero)
isalpha and such functions use int instead of char because int is big enough to hold characters and all also the value EOF(end of file).
Overlap is when two memory areas share bytes, it becomes a problem when copying memory areas when the source area is prior to the destination are.		
toupper uses Int as argumnet and return value, so it can handle "EOF", data type char cannot handle EOF since it is 4bytes.
		EOF is a value of no particular data type, it represents the end dof a file.
strchr uses int argument purely for historical reason, strchr existed when C had no protoype when declared and libc function's declarations arguments had not data types.so, any function argument with no data type gets promoted to int(which still exists to this day) and they kept it that way.

Why is there is such thing as signed and unsigned char ? 
why strncmp an memchr use unsigned char  ?
why does memchr uses unsigned char in comparison instead of char ?
what is the roel of pointer types ?	
why nil gets printed instead of null in memchr?

[C language]
lvalue = left-hand value
rvalue = right-hand value
long, short = these are qualifiers, not data types. they are usually used with integer data types such as: int and float.
		data types are usually ommited when using qualifiers(long long = long long int)
character constants are not of type char, they are promoted to int [sizeof('a') == sizeof(int)]
=== making the library===
we use ar (which is an archiving tool)
we have to use the flags (rc) with it to rell it what operations to run
	ar -rc lib.a objecfile.o
r: add object files (or replace them) to lib.a
c: create the archive lib.a
=== removeing files rm ====
when removing files, we use "-f" flag = it does not show the error if the file to be removed does not exist

[gdb]
gdb is a tool that helps you investigate seg fault
	run < input.txt => this will run the program using input from the text file "input.txt"

[printf]
variadic functions = functions that can take changing(non-fixed) number of arguments of unkown type.
ellipses == ... 
	it's the syntax of a variadic function. example => void func(int x, char c, ...)
[README.md]
	# this will display the text bigger (like an h1)
	> grayed out text
[File descriptor]	
	File descriptor is non negative integer, it works as process-unique identifier for a specific file.
	-Use fileno(file) to print the file descriptor of a file.
	-integers 0, 1 and 2 are reserved for the standard streams input, output and error.
	-Each process has its own fd table, 0, 1 and 2 are reserved which makes the table start from the integer 3.
	-the process speaks to the fd which speaks to the shell
	-Each peripheral with your pc is represented as a file (device file) in the unix file system.
		[stdin, stdout, stderr] 
			-stdin(by default is the keyboard)
				its fd is 0
			-stdout(by default is the screen)
				its fd is 1
			[redirection]
				*you can redirect the standard input and output to files
					example of stdout redirection:	ls (this is a normal example of stdout) / ls > file.txt (is an example of stdout redirection)
[get_next_line]
	[static variables]
		-They are only initialized once.
		-"normal" local variables are destroyed when their scope(function) is destroyed
					 
[vim]
	-copy for one file to another:
		:e nameoffile
	-remove first two charactes from each line:
		:%s/^..// (% = every line, ^.. = first two characters, / = replace with empty string)
	-add tab to each line:
		:%s/^/\t/
	-move cuurent line a certain number(in this example two lines) of lines
		:move .+2
	-redo 
		:redo or ctrl+r
	-remove all line starting from line 83
		:83,$d => the "$" is for the last line
	-save readonlyfile 
		:w !sudo tee %
	-set file name to vim window
		:set title
	-copy a line by number:
		:56y and then press "p" (this will copy line number 56)
	-replace all instances of a variable name (or just text in general) by another
		:%s/old_var/new_var/g
			g = is to replace all instances of that var, removing it will only replace the first instance
	(not really a vim command but seems appropriate here)
	-copy the content of a file to the clipboard
		cat main.c | xclip -sel clip
[virtualization] 

[extreme C]
source code = programming statments(c code)
COMPILATION PIPELINE
	preprocessor => compiler => assembler => linker
		*each step is vital
header files are files that containe(among other things) functions declarations
	functions definitions are not included in header files
	a collection of header files alongside source code files is a library
INITAILLY, in every c program, 3 types of files are involved:
	1.header file (which containes the function declaration among other things)
	2.source file that contains the functions defintion
	3.source file that contains the main function where the program starts(main)

1.[preprocessor]
	-removes comments
	-handles directives
	-literally copies and paste the content of the header files specified
	result: a single file that has a block of code that contains header files
			 content alongside the c code you wrote
			 (translation unit aka compilation unit .i format)
	run: gcc -E file.c => to get the translation unit
2.[compilation]
	-converts translation unit into assemby code
		-assembly is different from cpu to another(host/target architecture)
	run: gcc -S file.c => to get the assembly code
	outputs a file with the extension .s
3.[assembly]
	-converts assembly code into machine code (object file)
	run: gcc -c file.c to do the above three processes and get an object file
4.[linker]
	-creates the excutable(.out in unix or .exe in windows)
		it links the object file of the c code we wrote with the object 
			file of c code that has the functions's definition.
			
compiler
	how most compilers convert the same c code into the assembly of the target cpu
	compilers use a two steps operation to convert c code(translation unit) into assembly of target cpu
		frotend: archtecture independent(can be done in any cpu)
			turning translation unit into AST(abstract syntax tree)
				AST is a data structure that any programming language can understand
					hence the word abstract(maybe)
		backend: architecture dependent  
assembler
	there are two things that control the object file format 
		1.hardware (architecture)
		2.OS
	for example:
			MACH-O is the Object file format for MAC OS
			ELF is the object file format for linux
The entry point of a c program is the main function
	the entry point of an object file is platform deprendent
types of object files:
	1.relocatable object files
		.o extension: contain machine code
	2.executable object file
		.out contains machine code ready to excute
		it has multiple relocatable object files


MEMORY
	garabage collector is a mempry component that is responsible for deallocation
	In c, there is no such thing as garbage collector unlike languages like java
		and c#
	when an excutable object file is running, it is called a process.
	a process has two memory layouts
	a static memory layout and a dynamic memory layout
		1.static memory layouts of a porcess come from the excutable object file
		2.dynaimc memory layout of same process is built while process is loading
	Static memory layout
	run: size -m ex4_2-macos.out => to get static layout
		bss segement
			reserved to host uninitialized global variables and global 
				variables set to 0
		data segement
			reserved to host initialized global variables set to a non zero value
		text segement
			reserved for code you wrote
	dynamic memory layout (DML)
		when a process is runing, a program called the loader start the excution
			by first, forming the dynamic memory layout.
		it forms DML by copying the static memory layout and adding two more 
			segements		
		in addition to the static memory layout(bss, data, text), 2 more segments
			are added: stack and heap
[153 as explained before]


[memchr]
	why does it use int as second argumnet ?
		For historical reasons, memchr exist where there as no such thing as prototype, void *memchr(); /* non-prototype declaration */
			so every argument got implicit promotion.(char => int)
			for the sake of legacy libraries that used memchr in that form not breaking, they kept it.
	why unsigned char ?
		char => to compare each byte
		unsigned => 
[memcmp]
	why unsigned?
		portability, the signdness of char is machine dependent which can cause problems MAYBE.
	why that second if statement ?
		if n == 5 and str1= "hellox" str	2="helloy" 
[memcpy]
	why unsigned?
[memmove]
	why unsigned ?
	handles overlap => when to memory areas have common bytes
		ex: abcd => src
		      cdef => dst and len == 4	
[memset]
	why int ?
		same as memchr
	why unsigned ?

[ft_putchar_fd]
	what is a fd ?
		A non negative integer that act like a handle to a file in each process.
		Each process has a fd table, 0, 1, 2 are reserved to stdin, stdout, stderr.
		stdin refers the default output stream...usually terminal.
[putnbr]
	recursion ?
		function calling itself.
[is...]
	why they use int as argument ?
		to include EOF which is 4 bytes
[atoi itao]
	Implicit type conversion

[strchr strrchr]  
	why uses int ?
		same as memchr
	the char type cast is for 1024

[strlcat]
	test strlcat
	change strlcat

[ifndrf direcetive]
	header guard so that the header does not get included more than once.  



 	ask OBJS = $(SRCS:.c=.o)
*Variadic functions are functions that accept non-fixed number and different data types
*Macros are just pieces of codes that are stored somewhere and are pasted in preprocessing
	most languages don't have preprocessers, it's known to exist in C.

ar -r => create archive if it does not exist, add new files or replace chhanged files
ar -c => does the job silentely without printing informational message
rm -f => do not show confirmation question (create a file with 444 and remove it) and do not show "file does not exist" if file does not exist and you try deleting
rm -r => this flag needed to delete directories and subdirectories
(...) epilipse => syntax used by functions and macros to denote variable number of arguments
substituotion makefile => replaces the suffixe .c to .o
		the compilation => there an implilcit rule that commpiles
CFLAGS 	=> changing it would make it not compile with those flags
		IT is a variable used by implicit rules
Macros are just pieces of code that are replaced by the preprocessor.
	#define test 4 => will replace all occurences of test by 4.
	Macros and functions are similar in the fact that they encompass code to be used later.
the header guards #ifndef #define are macros 
va_list is a type just like an int and char are types
va_start
	it initializes ap meaning it prepares to be used by va_arg and va_and
	the second argument (last known parameter in the function) is then used to access the other arguments
va_arg
	a macro
	in a first invocation, it returns the argument after the last known argument and so on and on in each invocation
va_end 
	a macro
	signals that you are finished with va_list and we don't need to access any argument.
	it does clean up

unsigned int => int type that only represents 0 and postive integers 
		since it can't hold a positive number, which is represneted in the first byte. 
arhcive contains the object files of the compiled source code.
%i and %d are similar except that %i can print integers using their octal and hexadecimal representations 
[born2beroot V2]
[Signature]
	- A hexadecimal(base 16 number that uses alphabets to represent numbers beyond 9) which is a unique ID used to verify the authenticity of data.
	- Shasum is a tool that generates such signatures by the command "shasum file", and a minor change in the file would change the signature.
	- It is used as a way to establish trust and security, with it you can verify if the vdi was altered in some way, someone could replace the image for example.
	- It is also used by OS developpers to verify the authenticity of ISO files.
	!!!!! TODO: Verify the need for signature by doing. (sign it => change files in the os => check the signature, it should be changed)

[Virtual machine]
	- Virtualization: Creating the virtual version of physical system, in this case it is a Computer with its operating system.
	- Another example of virtualization is Storage Virtualization which is taking multiple physical storage devices and making a virtual storage pool out of them.
	- A vm is virtual computer.
	- It works exactly like a physical computer, it essentially a bunch of files like configuration file and disk image(usually an ISO) that gets handled by 
		software like virtualbox, it is completely seperate from the host machine.
	- It uses:
		* Running multiple servers in the same hardware.
		* Trying and using other operating systems.
		* OS and low level development.
		* Cybersecurity analysis and training.
	- The major difference between rock and debian is that:
		* Debian is easier to setup than rocky.
		* Debian was created as a general purpose OS suitable for a lot of use cases such as: servers, desktops and other use cases...
		* Rocky was created heavily to be used as in servers, it was also created as a replacement of centOS in mind.
		* CentOS's change of policy pushed the need to create rocky os, one of the changes that push them was lack of LTS.
		* The primary goal of development infleunces the development process, debian might focus on desktop environement more than rocky and focus less on 
			Security and provide LTS.
		* Debian uses APT and rokcy uses yum, this is a basic difference among many others.
	- APT (advanced package tool) a tool to manage(install packages, update them, remove them) packages and software. it just makes the package installation 
		process much easier.
		* apt and aptitude are pretty much the same thing, they are both package managers, what aptitude has that apt does not is the text based UI, and apt
			is used by aptitude.
				(run "aptitude" alone).
	- APPARMOR is a linux security application, it used to sandbox apps meaning define which ressources those apps have access to, the goal is to give apps 
		the minimum previlige possible.
		* it is like sudo but for apps instead for users.
		Example: 
			- Prevent a compromised website from accessing the files of another if they are in the same server.
			- Why would you give a game the access to the laptop camera when it does not need it.
		!!!!!!TODO: go more into that first example 
	- Password policy
		Advantages:
			Security i the main advantage of strict password policy.
		Disadvnatages:
			Forgetting the password and risking getting locked out is tha main disadvantage.
	!!!!!!TODO: The advantage and disadvantge of the that password policy implemntation.
	- LVM
		* It is a type of virtualization, Storage virtualization.
		* Enables you to partion your storage devices, An example is allocating different partitions for the home directory and logs directory, putting them
			in the same partition will prevent loggin in case that partition got full, it is also useful to use it to seperate the root directory and 
			the home directory to avoid problems.
		* Scalibility, Using LVM allows to scale up your storage without the need to move data, backup tha date or take the system down, you can literaly 
			hook up the new storage device and start working.
		*Backup: LVM uses snapshots, with it you back up your data at point in time. 
		* non linear resizing opposed to classical partitions.
	- SUDO
		Sudo is a program that temporarily gives users root previlege.
		Why the need for sudo ? different users need different previlges, a system admin has to have root access to better manage the system.
		but why not just be root all the time ? why do we need sudo and its temprarily access ? to prevent malicious programs from compromising the system 
			and prevent accidents.
		* Spoody example.
	- UFW
		* UFW is A program that works as a frontend for netfilter firewall, it makes it easier to use.
		* Firewall: A program that monitors network traffic, allowing or denying dat packets based on pre defined rules.
		Example: Allow ssh access from a specific IP address only.
			 Block your website access from a specific country or IP.
			 Students not having access to school's website from inside the school.
		* Ports are just numbers that are associated with a certain service in the server, for example, port 22 is associated with SSH access, port 443 is
			associated with HTTPS... it is a way for the server to organize itself and these services.
			- You type google URL in the browser, it gets turned into an IP address and a port associated with HTTPS or http, the server evaluate which 
			service is asscoiated with that port, it then verify if you have access to that service through that port and act accordignly.
		* Not all ports are associated with a service. 
	- SSH
		* A program that allows you to connect to computer/server and execute commands in that machine remotely in a secure way.
		* sys admins use it to troublshoot servers, send and recieve files to be physically where the server is.
		* its advantages:
			- Encrypting data.
			- Authentication.
		!!!!!!TODO: go a bit more into how its advantages work.
	- cron
		* A program that enables you to run shell commands periodicaly and automatically.
		* Its uses:
			- Periodically Backup the system.
			- Periodically update thes system. 
			- Periodacilly Send reports about the current state of the server or website, or send emails in case of problems.
		* Script Output:
			- 
		!!!!!!!TODO: understand how it works better especially those cron commands, and understand those outputs and their commands.

