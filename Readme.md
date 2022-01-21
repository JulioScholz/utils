# Utils
---
### Git
- [Nice git tutorial for begginers](https://rogerdudler.github.io/git-guide/) 
- Git init
`echo "# name" >> README.md`
`git init`
`git add README.md`
`git commit -m "first commit"`
`git branch -M main`
`git remote add origin https://github.com/JulioScholz/utils.git`
`git push -u origin main`
- Others
`git status`
`git fetch`
### RegEx
- Find all non empty lines with blank spaces at the end
    `([^ \t\r\n])[ \t]+$`

### Bat File
- Create a bat file to change the power profile on windows
    - Launch RegEdit and navigate to:
        - HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Power\User\PowerSchemes
    - Get the GUID (something like a1841308-3541-4fab-bc81-f71556f20b4a)
    `powercfg -s insert_GUID_here`