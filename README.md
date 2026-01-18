# git-release

Minimal tool to create and publish Git release tags following the vX.Y.Z format.

```bash
# Quick install
mkdir -p ${HOME}/.local/bin
wget -qO ${HOME}/.local/bin/git-release https://github.com/ObNitram/git-release/releases/latest/download/git-release
chmod +x ${HOME}/.local/bin/git-release
```

## Usage

- From the repository root: `git release`
- Select release type: patch, minor, major, or cancel
- Confirm the new version
- The script creates and pushes the new tag

### Multi-project support

For repositories with multiple projects (monorepos), you can specify the project name as an argument:
`git release <projectname>` will create a tag with the following format `<projectname>-vX.Y.Z`

## Example
```
$ git release 
    📦 Current version: v0.0.0
    Select release type:
    1) patch
    2) minor
    3) major
    4) cancel
    #? 2
    🚀 Creating new release: v0.1.0
    Confirm? (y/N): y
    Enumerating objects: 6, done.
    Counting objects: 100% (6/6), done.
    Delta compression using up to 20 threads
    Compressing objects: 100% (4/4), done.
    Writing objects: 100% (4/4), 560 bytes | 560.00 KiB/s, done.
    Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
    remote: Resolving deltas: 100% (1/1), completed with 1 local object.
    To github.com:ObNitram/git-release.git
    * [new tag]         v0.1.0 -> v0.1.0
    ✅ Release v0.1.0 created and pushed successfully!
```

## Installation
It's a single script file:
- Download the `git-release` script from the repository.
- Make it executable: `chmod +x git-release`
- Place it in your PATH

It relies on the fact that if git does not find a command, it will look for a script named `git-<command>` in your PATH.
So you can now run `git release` from any git repository.


You can use the following commands to install it:
```bash
mkdir -p ${HOME}/.local/bin
wget -qO ${HOME}/.local/bin/git-release https://github.com/ObNitram/git-release/releases/latest/download/git-release
chmod +x ${HOME}/.local/bin/git-release
```



## Dependencies
- git

## License
- MIT License
- See the repository `LICENSE` file.
