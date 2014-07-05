# smartos-munin-plugins

Modified munin plugins to work in an SmartOS zone. This repository is created
because of not working or wrong configured munin plugins, for example wrong
default shell for executing the script.

To get that working I easily replace all existing plugins in
`/opt/local/lib/munin/plugins` with the content of the repository. Be careful
because this will overwrite existing plugins.

All begin with a simple replace `#!/usr/xpg4/bin/sh` with `#!/usr/bin/bash`.
This allow you to use `plugin.sh` with the bash function `local`.
