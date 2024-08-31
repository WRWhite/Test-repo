# Test-repo
Test repository for training
Started a new repo called Test-repo  

repo init https://github.com/WRWhite/Test-repo  
Note the revision is the commit number in the default.xml  


Note that comments in default.xml are not support so will annotate here

<?xml version="1.0" encoding="UTF-8"?>
<manifest>

  <default sync-j="2"/>

  
  <remote name="WRWhite"           fetch="https://github.com/WRWhite"/>
 
 <project
    remote="WRWhite"
    name="Test-repo"    // Add to fetch in order to clone ie "git clone https://github.com/WRWhite/Test-repo
    path="Test-repo"    // Directiry on target device
   revision="master"    // branch, tag or commit hash
  />
  
  <project
    remote="WRWhite"
    name="ScratchPad"
    path="ScratchPad"
    revision="033941b0d11de451799ffe179032e51afffcc6d0"
  />

</manifest>
