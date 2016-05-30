# docker-node
Adds common `npm` build dependencies to the [official Node.js Docker image](https://hub.docker.com/r/library/node/)

## Organization
Currently the `master` branch is tracking nodejs current, or the `6.x` line:

| Branch | Release type | Versions | Latest tag |
| ------ | ------------ | -------- | ---------- |
| master | current      | 6.x      | 6.1.0      |
| 4.4    | LTS          | 4.4.x    | 4.4.5      |

## Adding new versions (Triggering an image build in Docker hub)
Image tags mirror git tags.  For example:

```
[4.4 branch] tags: [4.4.4]
/
/Dockerfile
/README.md
```
Where the Dockerfile is for nodejs `4.4.4`.

Creating the above branch, tagging HEAD with `4.4.4`, and pushing both will trigger a build.
