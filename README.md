# github-experience  
### 2022.8.1修改repository语言  
----------------------------------------------------------------------------------------------------------------------------------------------  
<!------------------------------------------------------------------------------------------------------------------------------------------->
 | Git attribute                                  | Defined in            | Effect on file                                                  |
 |:-----------------------------------------------|:----------------------|:----------------------------------------------------------------|
 | `linguist-detectable`                          | [`languages.yml`]     | Included in stats, even if language's type is `data` or `prose` |
 | `linguist-documentation`                       | [`documentation.yml`] | Excluded from stats                                             |
 | `linguist-generated`                           | [`generated.rb`]      | Excluded from stats, hidden in diffs                            |
 | `linguist-language`=<var><ins>name</ins></var> | [`languages.yml`]     | Highlighted and classified as <var><ins>name</ins></var>        |
 | `linguist-vendored`                            | [`vendor.yml`]        | Excluded from stats                                             |
<!------------------------------------------------------------------------------------------------------------------------------------------->  
example：  
.gitattributes  
*.SchDoc linguist-detectable  
*.PcbDoc linguist-detectable  
*.PrjPcb linguist-detectable  
*.SchLib linguist-detectable  
*.PcbLib linguist-detectable  
*.Cam linguist-detectable  
*.GML linguist-detectable  
*.schdoc linguist-detectable  
*.pcbdoc linguist-detectable  
*.schdoc linguist-language=SchDoc  
*.pcbdoc linguist-language=PcbDoc  
*.GML linguist-language=PcbDoc  

> 修改VScode Git路径：打开设置，输入git.path，修改json文件   
> 使用linux style 例如：C:/mysoft/Git/Git/bin/git.exe  
