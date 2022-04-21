# Vforces

Hi! Here's a list of solutions to Codeforces problems written in V for demonstrational purposes.

## Setup
I use VS Code with an awesome **acmX** [extension](https://marketplace.visualstudio.com/items?itemName=marx24.acmx) on Ubuntu 20.04. Here's their [GitHub](https://github.com/mfornet/acmx)
 
1. Install **V** ([link](https://github.com/vlang/v#installing-v---from-source-preferred-method))
1. Symlink the compiler ([link](https://github.com/vlang/v#symlinking))
1. Get Competitive Companion for [Chrome](https://chrome.google.com/webstore/detail/competitive-companion/cjnmckjndlpiamhfimnnjmnckgghkjbl) or [Firefox](https://addons.mozilla.org/ru/firefox/addon/competitive-companion/).
1. In browser, go to
    * (*Chrome*) 
        * Extensions -> Competitive Companion -> Options
        * In `Custom ports`, type `10042`
    * (*Firefox*)
        * Add-ons and themes -> Competitive Companion -> Preferences
        * In `Custom ports`, type `10042`
1. Now, it will send the parsed problems to the port `10042`
1. Install VS Code ([link](https://code.visualstudio.com/))
1. Open terminal with `Ctrl` + `Alt` + `T`
1. Clone this repository
    ```sh
    git clone https://github.com/br4ch1st0chr0n3/vforces
    ```
1. Open it in VS Code
    ```sh
    code vforces
    ```
1. Go to Extensions (looks like blocks in the sidebar)
1. Type `acmX`, press on it, click `Install`
1. While on this extension page, click on the `gear icon` -> `Extension settings`
1. Scroll down until `Acmx › Template: Solution Path`
1. Paste `$HOME/.acmx/templates/sol.v` there. This will be the path to our template solution
1. Now, open terminal via `Ctrl` + `Shift` + `` ` ``
1. Copy the template `sol.v` from this repository into `~/.acmx/templates/sol.v`
    ```sh
    mkdir -p ~/.acmx/templates/ && cp sol.v ~/.acmx/templates/sol.v
    ```
    * Of course, you can edit this template as you wish
1. Let's add the configuration file for `V`:
    ```sh
    cp vlang.json ~/.acmx/languages/
    ```
    * Next time, if you want to edit it, open Command Palette with `Ctrl` + `Shift` + `P`, then type `acmx edit`, then choose `vlang`
    * IDK why but they need all commands to be split into separate strings.
1. Time to run our solutions! Open a Codeforces problem, say [1661D](https://codeforces.com/problemset/problem/1661/D)
1. Press on Competitive Companion extension
1. VS Code opens with full setup!
1. Open `sol.v`
1. Copy code from this repository, from `solutions/1661D.v` into this newly opened `sol.v`
1. While in `sol.v`, open Command Palette with `Ctrl` + `Shift` + `P`, type `ACMX: Run`
1. Tests passed!