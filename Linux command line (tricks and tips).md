# Linux command line tricks and tips
- Create dir and enter it:
`mkdir dirname && cd $_`
*`cd $_` retrievs the last argument of the previous command, while `cd !$` gives the last argument of previous command in the **shell history***
- Commands to work with history effectively:
`history | grep <search_string>`
`!<number>` *- to call line from history output*
`!!` *- to call last command (useful for commands which require sudo)*
CTRL+R *- for search in command history*
- Move to previous catalog:
`cd -`
- Home folder:
`~`
- Stacking folders:
`dirs -v` *- to see full stack*
`dirs -c` *- to clear stack*
stacked dirs can be accessed using `~<number>`
`pushd <folder name>` *- to put folder to stack*
`popd` *- to pull folder from stack*
- Exit terminal but leave all processes running
`disown -a && exit`
- Use less 
`less +F` *- to open file in follow mode (see updates in real time)*
CTRL+C *- to stop follow mode,* SHIFT+F *- to resume it*
- Use terminal shortcuts:
CTRL+A *- to move to the beginning of the line and* CTRL+E *to move to the end*
CTRL+K *- to cut everything after the cursor*
CTRL+Y *- to paste back*
CTRL+U *- to cut everything before the cursor*
CTRL+W *- to delete last word* 
