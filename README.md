# gitbook-plugin-get-pdf

在顶部左侧工具栏添加下载 PDF 链接，修复了 download-pdf-link 链接地址错误的问题。

## 下载该插件
```
npm install gitbook-plugin-get-pdf
```

## 使用该插件

### 多语言环境
```js
{
    "plugins": ["get-pdf"],
    "pluginsConfig": {
        "get-pdf": {
            "base": "http://pmglab.top/commandParser/",
            "prefix": "book",
            "label": {
                "en": "Download PDF",
                "zh": "下载 PDF"
            }
        }
    }
}
```

自动文件名格式: base/prefix_lang.pdf

例: 若在 en 语言下点击下载按钮，将打开 http://pmglab.top/commandParser/book_en.pdf 文件。

### 单语言环境
```js
{
    "plugins": ["get-pdf"],
    "pluginsConfig": {
        "get-pdf": {
            "base": "http://pmglab.top/commandParser/",
            "prefix": "book",
            "label": "下载 PDF"
        }
    }
}
```

自动文件名格式: base/prefix.pdf

例: 点击下载按钮，将打开 http://pmglab.top/commandParser/book.pdf 文件。

