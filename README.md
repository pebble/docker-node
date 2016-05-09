# docker-node
Adds common npm build deps to the official node.js Dockerfile

## Adding new versions (Triggering an image build in Docker hub)
Image tags mirror branch names.  For example:

```
[4.4.4 branch]
/
/Dockerfile - Dockerfile for node.js 4.4.4
/README.md - This README
```

Creating and pushing the above would trigger a build.  Master can store the latest stable Dockerfile.
