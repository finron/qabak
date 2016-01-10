1. q:list recently install software
a: http://helpdeskgeek.com/linux-tips/display-a-list-of-recently-installed-software-packages-in-ubuntu/
   core: vi /var/log/dpkg.log
   
2. q:copy file from client to server 
a:http://unix.stackexchange.com/questions/106480/how-to-copy-files-from-one-machine-to-another-using-ssh
   core:sshfs user@server.com:/remote/dir /home/user/test

3. pg-config-executable-not-found
a: see http://stackoverflow.com/questions/11618898/pg-config-executable-not-found
   core:sudo apt-get install libpq-dev python-dev

4. urllib3 from configuring SSL appropriately and may cause certain SSL connections to fail.
a: see http://stackoverflow.com/questions/29134512/insecureplatformwarning-a-true-sslcontext-object-is-not-available-this-prevent
	https://urllib3.readthedocs.org/en/latest/security.html#pyopenssl
	core:pyopenssl

5. find-out-library-version
http://superuser.com/questions/690306/find-out-library-version
	core: ldconfig -v | grep libnuma
	
6. postgresql ./configure error - readline library not found
http://www.postgresql.org/message-id/m3he1ypgmu.fsf@varsoon.wireboard.com
	core:  This is the runtime part of the library, but you need the headers to
compile, which are in the -devel package.

7. man useradd passwd groupadd 'config vim'

8. pgadmin3  No protocol specified Error: Unable to initialize gtk, is DISPLAY set properly?
a: see http://postgresql.nabble.com/Unable-to-initialize-gtk-is-DISPLAY-set-properly-td5112938.html
 core: start with root
 
9. vimwiki unknown function 
a: see http://stackoverflow.com/questions/25755600/vim-cant-get-vundle-plugin-to-work-unknown-function
    core:set nocompatible
	set rtp+=$HOME/.vim/bundle/vundle
	let path='$HOME/.vim/bundle'
	call vundle#rc('$HOME/.vim/bundle')
	
10. reset git passphrase
    link first http://stackoverflow.com/questions/6565357/git-push-requires-username-and-password
    link:https://help.github.com/articles/set-up-git/
    
11. show git config list
    link: http://stackoverflow.com/questions/12254076/show-git-config
    core:git config --list (shortest -l)

12. Ubuntu Missing add-apt-repository command
    link: http://lifeonubuntu.com/ubuntu-missing-add-apt-repository-command/    core: sudo apt-get install software-properties-common python-software-properties
    note: in ubuntu server 14.04 without first cannot get solved
