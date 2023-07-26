# OSX-VIMR-ANYWHERE

Like [vim-anywhere][1], but for neovim with Vimr GUI for macOS.

Also current implementation works n times faster.

[1]: https://github.com/cknadler/vim-anywhere
[2]: https://github.com/koekeishiya/skhd
[3]: https://github.com/qvacua/vimr

## Installation

This implementation depends on 2 apps: [vimr][3] and [skdh][2].
Skhd is a tool to set up hotkeys (and it work faster than the solution from the original vim-anywhere).

```bash
# install vim client
brew install vimr

# setup skdh
brew install skhd
brew services start skhd
touch ~/.skhdrc
echo 'shift + alt - v : bash ~/osx-vimr-anywhere/run.sh' > ~/.skhdrc 

# copy repo with the script
git clone https://github.com/Liverm0r/osx-vimr-anywhere.git ~/osx-vimr-anywhere
```

Typing shift+alt+v opens vim buffer. Exit with `:x` and you will have your previous app opened and content put in the clipboard.

## Legacy installation

Check the instatuction from the first [commit](https://github.com/Liverm0r/osx-vimr-anywhere/commit/6d9a797184f35fe4bd12b7a8df74c72fd128754f)

## Customization

This app is just one script with several lines of code — you will handle it, I promice ;)

Change `VIM` to path of the vim client you want to use (result of `which vimr`).

    VIM=/opt/homebrew/bin/vimr

## License

Copyright 2022 Artur Dumchev

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the
License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "
AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific
language governing permissions and limitations under the License.
