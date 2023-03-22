The scripts `cleanup.sh` & `reset.sh` are meant to help cleaning up the files created by the LaTeX compilation:

- `cleanup.sh` removes all auxiliary files that LaTeX generates during compilation, that are located in the `course/build` directory. It also moves the generated `.pdf` file to the main `course` directory.

- `reset.sh` removes all files that LaTeX generates during the compilation, so the `.pdf` file is also included in this case.

Since it could be useful at any given moment in time, you can run the scripts directly from gvim using the `:!` prefix. For example you can use `:! bash my_script.sh` inside gvim to execute `my_script.sh`. You just need to make sure that the script is specified with the correct path, relative to the directory of the current buffer from which you are executing the command.

You can also map a key to execute the command that runs the scripts, so that you don't have to type it every time. You can for example map a key inside your `.vimrc` configuration file, so that it is always available.
