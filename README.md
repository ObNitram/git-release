# git-release

Minimal tool to create and publish Git release tags following the vX.Y.Z format.

## Usage
- From the repository root: `./git-release`
- The script creates an annotated tag and pushes it to the configured remote.
- If the script is in your PATH, you can run it directly with `git release`


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
- Make the script executable: `chmod +x git-release`
- (Optional) Create a hard link in your PATH : 
   `ln "$(pwd)/git-release" "$HOME/.local/bin/git-release"`


## Dependencies
- git

## License
- See the repository `LICENSE` file.