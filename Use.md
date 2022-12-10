# 转换说明

## markdown 转 html
```
pandoc README.md -o test.html
```

## markdown 转 word
```
pandoc -f markdown_github -t docx ./README.md -o test.docx 
```