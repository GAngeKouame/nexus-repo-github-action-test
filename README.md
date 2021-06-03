<!--![nexus-repo-github-action-test](https://github.com/bhamail/nexus-repo-github-action-test/workflows/Go/badge.svg)-->
<a href="https://github.com/bhamail/nexus-repo-github-action-test/actions?query=workflow%3AGo"><img src="https://github.com/bhamail/nexus-repo-github-action-test/workflows/Go/badge.svg" alt="nexus-repo-github-action-test"></img></a>

Nexus Repository Publisher GitHub Actions play project
===========================

Runs the [nexus-repo-github-action](https://github.com/sonatype-nexus-community/nexus-repo-github-action).

You can run a local build using the [act](https://github.com/nektos/act) project. e.g.:
```shell
$ act
[Go/Build] 🚀  Start image=catthehacker/ubuntu:act-latest
[Go/Build]   🐳  docker run image=catthehacker/ubuntu:act-latest entrypoint=["/usr/bin/tail" "-f" "/dev/null"] cmd=[]
[Go/Build]   🐳  docker cp src=/Users/bhamail/sonatype/community/go/nancy-gh-action-test/. dst=/github/workspace
[Go/Build] ⭐  Run Set up Go 1.x
[Go/Build]   ☁  git clone 'https://github.com/actions/setup-go' # ref=v2
[Go/Build]   🐳  docker cp src=/Users/bhamail/.cache/act/actions-setup-go@v2 dst=/actions/
| Setup go stable version spec ^1.16
[Go/Build]   💬  ::debug::isExplicit: 
[Go/Build]   💬  ::debug::explicit? false
...
| ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
| ┃ Summary                     ┃
| ┣━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━┫
| ┃ Audited Dependencies    ┃ 0 ┃
| ┣━━━━━━━━━━━━━━━━━━━━━━━━━╋━━━┫
| ┃ Vulnerable Dependencies ┃ 0 ┃
| ┗━━━━━━━━━━━━━━━━━━━━━━━━━┻━━━┛
[Go/Build]   ✅  Success - Scan with specific Nancy version
```

ToDo
----
* ~~Done: Replace the commit hash below with a reference to either a release version or the `main` branch
in `.github/workflows/go.yml`:~~
  ```yaml
  uses: sonatype-nexus-community/nexus-repo-github-action@811b6670e343fc48fde273906404adaac9bd3885
  ```
