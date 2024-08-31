# Test-repo
Test repository for training. This repo contains the default.xml file for use with the Google repo utility   
Clone with the following command  
```
repo init https://github.com/WRWhite/Test-repo  
```

Note that comments in default.xml are not support so will annotate here instead

```
<?xml version="1.0" encoding="UTF-8"?>
<manifest>

  <default sync-j="2"/>

  
  <remote name="WRWhite"           fetch="https://github.com/WRWhite"/>
 
 <project
    remote="WRWhite"
    name="Test-repo"    <!-- Add to "fetch" in order to clone ie "git clone https://github.com/WRWhite/Test-repo"
    path="Test-repo"    <!-- Directiry on target device
   revision="master"    <!-- Branch, tag or commit hash
  />
  
  <project
    remote="WRWhite"
    name="ScratchPad"
    path="ScratchPad"
    revision="033941b0d11de451799ffe179032e51afffcc6d0" <!-- This is a commit hash
  />

</manifest>
```
