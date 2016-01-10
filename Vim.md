-  :noh  to the backslash key. 

	To reenable the highlighting, just hit   n 

-  set vim default git editor

	git config --global core.editor "vim"

-  find the file and delete command

	find . -name *.png | xargs rm -fr

---- 
[copy with no auto indent](http://stackoverflow.com/questions/2514445/turning-off-auto-indent-when-pasting-text-into-vim)

:set paste or "+p

----
[select all and copy](http://stackoverflow.com/questions/15610222/how-to-select-all-and-copy-in-vim)

:%y+ or gg"+yG
