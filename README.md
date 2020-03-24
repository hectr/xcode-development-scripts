# xcode-development-scripts

⚠️ **WARNING:** Quick & dirty shell scripts. You should probably stay away.

## Suggested installation process

**1. Open terminal:**

`⌘` + `␣`, `terminal.app` then `⏎`

**2. Change directory to your repository root:**

**`$`**`cd /yor/repo/path`

**3. Copy this repository contents to `Vendor/Scripts` directory:**

**`$`**`mkdir -p "Vendor/Scripts"; export repo_path=$( pwd ); cd $( mktemp -d ); curl https://raw.githubusercontent.com/hectr/xcode-development-scripts/master/root-directory-path > root-directory-path ; curl https://raw.githubusercontent.com/hectr/xcode-development-scripts/master/download-github-repository > download-github-repository; bash download-github-repository --output_directory="${repo_path}/Vendor/Scripts"; cd "${repo_path}"`

**4. Track the `Vendor/Scripts` directory:**

**`$`**`git add Vendor/Scripts`

**`$`**`git commit -m "Add xcode-development-scripts"`

**`$`**`git push origin HEAD`

## Suggested update process

To keep the scripts updated you can use the included `download-github-repository` script.

**If you followed the suggested installation process**, simply execute it from Finder (double-click).

**If you copied the scripts to a custom location inside your repository**, you will need to execute the script passing the custom location path:

**`$`**`path/to/your/custom/location/download-github-repository --output_directory="path/to/your/custom/location/"`

## License

**xcode-development-scripts** is available under the MIT license. See the LICENSE file for more info.
