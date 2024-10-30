# 转换说明

## macos安装pandoc
```zsh
brew install pandoc
```

## markdown 转 html
```zsh
pandoc README.md -o test.html
```

## markdown 转 word
```zsh
pandoc -t docx ./README.md -o test.docx 
```