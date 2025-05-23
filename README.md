### ℹ️ About
This is a repo containing an action that lets you build any packages from [stal-ix/ix](https://github.com/stal-ix/ix) quickly on Github Actions.

### 🪄 Quickstart
1. [Fork this repo](https://github.com/pkgforge-community/stalix-pkger/fork)
2. Go to Actions & Start filling Inputs
> ![image](https://github.com/user-attachments/assets/b748d788-db23-4efa-a747-1d917a35570a)
> 1. Package Name is the full name like in this file: https://github.com/stal-ix/ix/blob/main/pkgs/die/scripts/dump.json (Examples: `bin/wget/2`, `bin/vim` etc)<br>

> [!NOTE]
> - This must resolve to a `ix.sh` script from: https://github.com/stal-ix/ix/blob/main/pkgs/${pkg_name}/ix.sh
> - Example: `bin/7z` --> https://github.com/stal-ix/ix/blob/main/pkgs/bin/7z/ix.sh

> 2. Choose Host, by default it will run on `x86_64-Linux`
> 3. Enable Debug Mode
> 4. Publish as Github Release
3. Run your workflow & wait for it to finish
4. If successful, check the releases section
---

### 🧰 Technical Details
#### Dockerfiles:
- https://github.com/pkgforge/devscripts/blob/main/Github/Runners/alpine-ix.dockerfile
- https://github.com/pkgforge/devscripts/blob/main/Github/Runners/debian-ix.dockerfile
#### Runners:
- https://github.com/orgs/pkgforge/packages/container/package/devscripts%2Falpine-ix
- https://github.com/orgs/pkgforge/packages/container/package/devscripts%2Fdebian-ix
- & More: https://github.com/pkgforge/soarpkgs/issues/191
