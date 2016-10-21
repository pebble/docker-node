# docker-node
Adds common `npm` build dependencies to the [official Node.js Docker image](https://hub.docker.com/r/library/node/)

## Organization
Currently the `master` branch is tracking nodejs current, or the `6.x` line:

| Branch | Release type | Versions |
| ------ | ------------ | -------- |
| master | LTS          | 6.9.x    |
| 4.6    | LTS          | 4.6.x    |
| 4.5    | LTS          | 4.5.x    |
| 4.4    | LTS          | 4.4.x    |

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
