# Linux command line tricks and tips
- **Create dir and enter it:**
  `mkdir dirname && cd $_`
  *`cd $_` retrievs the last argument of the previous command, while `cd !$` gives the last argument of previous command in the **shell history***

- **Commands to work with history effectively:**
  `history | grep <search_string>`
  `!<number or command>` *- to call line from history output*
  `!!` *- to call last command (useful for commands which require sudo)*

  `!*` - *to get all arguments from previous command* (`!:1 ... n` *to get specific argument*, `$` *and* `^` *are last and first argument*)

  CTRL+R *- for search in command history*

  `^<string to replace>^<replacement string>`- *will repeat previous command but with replaced string*

- **Move to previous catalog:**
  `cd -`

- **Home folder:**
  `~`

- **Stacking folders:**
  `dirs -v` *- to see full stack*
  `dirs -c` *- to clear stack*
  stacked dirs can be accessed using `~<number>`
  `pushd <folder name>` *- to put folder to stack*
  `popd` *- to pull folder from stack*

- **Exit terminal but leave all processes running**
  `disown -a && exit`
  `nohup <command> &` - *to continue command execution in background after closing terminal*

- **Use less** 
  `less +F` *- to open file in follow mode (see updates in real time)*
  CTRL+C *- to stop follow mode,* SHIFT+F *- to resume it*

- **Use terminal shortcuts:**
  CTRL+A *- to move to the beginning of the line and* CTRL+E *to move to the end*
  CTRL+K *- to cut everything after the cursor*
  CTRL+Y *- to paste back*
  CTRL+U *- to cut everything before the cursor*
  CTRL+W *- to delete last word* 

- **Search for string in all files**
  `grep -ri <string to find> <path>` - *where **r** means recursive search and **i** means ignoring case*

- **Search string in man pages**

  `apropos <string>`
