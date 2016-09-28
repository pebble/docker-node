# docker-node
Adds common `npm` build dependencies to the [official Node.js Docker image](https://hub.docker.com/r/library/node/)

## Organization
Currently the `master` branch is tracking nodejs current, or the `6.x` line:

| Branch | Release type | Versions | Latest tag |
| ------ | ------------ | -------- | ---------- |
| master | current      | 6.x      | 6.1.0      |
| 4.6    | LTS          | 4.6.x    | 4.6.0      |

## Adding new versions (Triggering an image build in Docker hub)
Image tags mirror git tags.  For example:

```
[4.6 branch] tags: [4.6.0]
/
/Dockerfile
/README.md
```
Where the Dockerfile is for nodejs `4.6.0`.

Creating the above branch, tagging HEAD with `4.6.0`, and pushing both will trigger a build.
