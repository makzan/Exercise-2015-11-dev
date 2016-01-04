#Basic Merge Conflict

You can use a graphical tool to resolve the conflict issue,you can run 
	git mergetool

whick fires up an appropriate visual merge tool and walks you through the conflicts:
	
	git mergetool
	This message is displayed because 'merge.tool' is not configured.
	See 'git mergetool --tool-help' or 'git help config' for more details.
	'git mergetool' will now attempt to use one of the following tools:
	opendiff kdiff3 tkdiff xxdiff meld tortoisemerge gvimdiff diffuse diffmerge ecmerge p4merge araxis bc3 codecompare vimdiff emerge
	Merging:
	index.html
	Normal merge conflict for 'index.html':
	{local}: modified file
	{remote}: modified file
	Hit return to start merge resolution tool (opendiff):

If you want to use a merge tool other than the default (Git chose opendiff in this case because the command was run on a Mac), you can see all the supported tools listed at the top after “one of the following tools.” Just type the name of the tool you’d rather use.

You can modify that message with details about how you resolved the merge if you think it would be helpful to others looking at this merge in the future – why you did what you did, if it’s not obvious.
