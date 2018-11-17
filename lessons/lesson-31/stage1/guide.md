## Docker Containers

**Contributed by: [Sudhishna Sendhilvelan](https://github.com/Sudhishna) and [Vinayak Iyer](https://github.com/vinayak-skywalker)**

---

## Part 1 - Docker Images and Containers

```
docker --version
```
<button type="button" class="btn btn-primary btn-sm" onclick="runSnippetInTab('docker1', 0)">Run this snippet</button>

```
docker run hello-world
```
<button type="button" class="btn btn-primary btn-sm" onclick="runSnippetInTab('docker1', 1)">Run this snippet</button>

```
docker image ls
```
<button type="button" class="btn btn-primary btn-sm" onclick="runSnippetInTab('docker1', 2)">Run this snippet</button>

```
cat Dockerfile
```
<button type="button" class="btn btn-primary btn-sm" onclick="runSnippetInTab('docker1', 3)">Verify Output (Optional)</button>

```
docker build -t saltimage .
```
<button type="button" class="btn btn-primary btn-sm" onclick="runSnippetInTab('docker1', 4)">Run this snippet</button>

```
docker image ls
```
<button type="button" class="btn btn-primary btn-sm" onclick="runSnippetInTab('docker1', 5)">Run this snippet</button>

```
docker run saltimage
```
<button type="button" class="btn btn-primary btn-sm" onclick="runSnippetInTab('docker1', 6)">Run this snippet</button>

```
docker container ls
docker container ps
```
<button type="button" class="btn btn-primary btn-sm" onclick="runSnippetInTab('docker1', 7)">Run this snippet</button>

```
docker container ls -a
```
<button type="button" class="btn btn-primary btn-sm" onclick="runSnippetInTab('docker1', 8)">Run this snippet</button>

```
docker pull busybox
```
<button type="button" class="btn btn-primary btn-sm" onclick="runSnippetInTab('docker1', 9)">Run this snippet</button>
