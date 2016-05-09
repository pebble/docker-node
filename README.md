# docker-node
Adds common npm build deps to the official node.js Dockerfile

## Adding new versions (Triggering an image build in Docker hub)
Image tags mirror branch names.  For example:

```
[4.4.4 branch]
/
/Dockerfile
/README.md
```
Where the Dockerfile is for nodejs 4.4.4.

Creating and pushing the above would trigger a build.  Master can point to the latest stable LTS Dockerfile.
