ePub 起始模版
================

http://github.com/wastemobile/epub-boilerplate

原始來源： http://javierarce.github.com/epub-boilerplate

ePub 起始模版是一份能幫您建置 ePub 格式、通過驗證，且完全符合 IDPF 標準的簡易模版。改製自 javierarce 的貢獻，並已將各內容對應設置為繁體中文。

## 如何使用

1. 取得模版：

        $ git clone git@github.com:wastemobile/epub-boilerplate.git

2. 編輯位於 **book** 目錄下的書籍內容。

3. 執行出版程序檔，會打包 ePub 電子書並使用 IDPF 驗證程式（目前版本 3.0b5）驗證一次：

## ePub 驗證

這流程使用了 epubcheck 驗證打包後的 ePub 書檔，執行前請確認系統已安裝了 Java，且執行路徑均已設置妥當。

        $ ./publish book.epub

## 書籍的結構

範例書檔包含下列檔案:

    ▾ book/
      ▾ META-INF/
          com.apple.ibooks.display-options.xml
          container.xml
      ▾ OEBPS/
        ▾ Images/
            cover.jpg
            image-01.jpg
            image-02.png
        ▾ Styles/
            style.css
        ▾ Text/
            acknowledgements.xhtml
            chapter01.xhtml
            chapter02.xhtml
            chapter03.xhtml
            cover.xhtml
            dedication.xhtml
            endnotes.xhtml
            foreword.xhtml
            frontmatter.xhtml
            introduction.xhtml
            toc.xhtml
          content.opf
          toc.ncx
        mimetype
        

## ePub 驗證

關於驗證程序，請參考這篇 <a href="http://blog.threepress.org/2010/12/16/running-epubcheck-on-your-computer/">詳細步驟解說</a>。

## 使用檢查程式（check script）驗證 ePub 電子書。

    $ ./check book.epub    

驗證程序目前版本為 EpubCheck version 3.0-RC-1。

## 格式

這程序目前沒有定義任何格式，作者或編輯可以參考這個 <a href="https://github.com/mattharrison/epub-css-starter-kit">ePub CSS Starter Kit</a>。行有餘力，會試著也將它改製成適合繁體中文電子書的起始格式，或是像 Twitter Bootstrap 那般易於修改與設置的格式起始模版。

## ePub → mobi（Amazon Kindle 電子書格式）

下面是將 ``.epub`` 轉成 ``.mobi`` 的簡易程序：

1. 下載 [KindleGen](http://www.amazon.com/gp/feature.html?ie=UTF8&docId=1000765211)。
2. 解壓檔案。
3. 拷貝 ``kindlegen`` 執行檔到 ``bin`` 目錄（或自行定義、加入至 $PATH 中的可執行路徑）。
4. 執行 ``./bin/kindlegen book.epub``。

## 一些有用的參考資源
      
* [EPUB 3.0 spec](http://idpf.org/epub/30)
* [Device compatibilty chart](http://wiki.mobileread.com/wiki/Device_Compatibility)
* [ePub CSS Starter Kit](https://github.com/mattharrison/epub-css-starter-kit)
* [ePub Validator](http://code.google.com/p/epubcheck)
* [UUID generator](http://www.famkruithof.net/uuid/uuidgen)
* [BISAC Subject Headings List](http://www.bisg.org/what-we-do-0-136-bisac-subject-headings-list-major-subjects.php)
* [Practical ePub metadata: Authorship](http://blog.threepress.org/2009/11/27/practical-epub-metadata-authorship/)
* [MARC Code List for Relators](http://www.loc.gov/marc/relators)
* [What Is EPUB 3? An Introduction to the EPUB Specification for Multimedia Publishing](http://shop.oreilly.com/product/0636920022442.do)
