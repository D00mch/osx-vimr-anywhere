# OSX-VIMR-ANYWHERE

Like [vim-anywhere](1), but for neovim with Vimr GUI for macOS.

[1]: https://raw.githubusercontent.com/cknadler/vim-anywhere

## Installation

Be sure to install vimr First

    brew install vimr

Then clone this repo into your `~/` directory, and install automator's quick-action: 

    mkdir -p ~/Library/Services; cp -R ~/osx-vimr-anywhere/VimRAnywhere.workflow ~/Library/Services   

Then select default keys to open vim from anywhere

    System Preferences —> Keyboard —> Shortcuts —> Services —> VimRAnywhere

## License

Copyright 2022 Artur Dumchev

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the
License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "
AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific
language governing permissions and limitations under the License.