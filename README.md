# xcode-development-scripts

⚠️ **WARNING:** Quick & dirty shell scripts. You should probably stay away.

## Recommended installation process

Just copy the scripts you want to use to some location in your git repository (e.g. `Scripts/`)

## Alternative installation process

**1. Open terminal:**

`⌘` + `␣`, `terminal.app` then `⏎`

**2. Change directory to your repository root:**

**`$`**`cd /yor/repo/path`

**3. Download this repository contents to `Vendor/Scripts` directory:**

**`$`**`mkdir -p "Vendor/Scripts"; repo_path=$( pwd ); cd $( mktemp -d ); curl https://raw.githubusercontent.com/hectr/xcode-development-scripts/master/download-github-repository > download-github-repository; bash download-github-repository --output_directory="${repo_path}/Vendor/Scripts"; cd "${repo_path}"`

**4. Track the `Vendor/Scripts` directory:**

**`$`**`git add Vendor/Scripts`

**`$`**`git commit -m "Add xcode-development-scripts"`

**`$`**`git push origin HEAD`

## Update process

To keep the scripts updated you can use the included `download-github-repository` script.

Execute it from Finder (double-click) and all the scripts will be updated to the last stable version.

Alternatively, you can **download the scripts to a custom location** with the `--output_directory=` parameter:

**`$`**`path/to/download-github-repository --output_directory="path/to/your/custom/location/"`

## License

**xcode-development-scripts** is available under the MIT license. See the LICENSE file for more info.
