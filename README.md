# git-release

Minimal tool to create and publish a Git release (tag + push) from a local repo.

Installation
- Make the script executable: `chmod +x git-release`
- (Optional) Copy to PATH: `cp git-release $HOME/.local/bin/git-release`

Usage
- From the repository root: `./git-release`
- The script creates an annotated tag and pushes it to the configured remote.
- If the script is in your PATH, you can run it directly with `git release`

Dependencies
- git

License
- See the repository `LICENSE` file.