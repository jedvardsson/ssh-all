ssh-all
=======

Bash utility to execute ssh command over a list of hosts.


Installation
============

Put the script in directory in your PATH, e.g. $HOME/bin.

	curl https://raw.github.com/jedvardsson/ssh-all/master/ssh-all > ~/bin/ssh-all


Examples
========

	$ ssh-all -h
	Run ssh command over list of hosts.
	
	Usage:
	
	ssh-all [options] [host...] -- [ssh-args]
	
		-h, --help              Shows this help.
	
	$ ssh-all host1.example.com host2.example.com -- "ls -A1"
	host1.example.com: .bash_history
	host1.example.com: .bash_logout
	host1.example.com: .bash_profile
	host1.example.com: .bashrc
	host1.example.com: .lesshst
	host1.example.com: .mysql_history
	host1.example.com: .ssh
	host1.example.com: .viminfo
	
	host2.example.com: .bash_history
	host2.example.com: .bash_logout
	host2.example.com: .bash_profile
	host2.example.com: .bashrc
	host2.example.com: .lesshst
	host2.example.com: .mysql_history
	host2.example.com: .ssh
	host2.example.com: .viminfo

