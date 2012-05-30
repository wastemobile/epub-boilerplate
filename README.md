ePub 起始模版
================

http://github.com/wastemobile/epub-boilerplate

原始來源： http://javierarce.github.com/epub-boilerplate

ePub 起始模版是一份能幫您建置 ePub 格式、通過驗證，且完全符合 IDPF 標準的簡易模版。改製自 javierarce 的貢獻，並已將各內容對應設置為繁體中文。

## 如何使用

1. 取得模版：

        $ git clone git@github.com:wastemobile/epub-boilerplate.git

2. 編輯位於 **book** 目錄下的書籍內容。

3. 執行出版程序檔，會打包 ePub 電子書並使用 IDPF 驗證程式驗證一次：

        $ ./publish book.epub

## ePub 驗證

這流程使用了 epubcheck 驗證打包後的 ePub 書檔，執行前請確認系統已安裝了 Java，且執行路徑均已設置妥當。

關於驗證程序，請參考這篇 <a href="http://blog.threepress.org/2010/12/16/running-epubcheck-on-your-computer/">詳細步驟解說</a>。

## 使用檢查程式（check script）驗證 ePub 電子書。

    $ ./check book.epub
    
## 格式

這程序目前沒有定義任何格式，作者或編輯可以參考這個 <a href="https://github.com/mattharrison/epub-css-starter-kit">ePub CSS Starter Kit</a>。行有餘力，會試著也將它改製成適合繁體中文電子書的起始格式，或是像 Twitter Bootstrap 那般易於修改與設置的格式起始模版。

## 一些有用的參考資源
      
* <a href="http://idpf.org/epub/30">EPUB 3.0 spec</a></li>
* <a href="http://wiki.mobileread.com/wiki/Device_Compatibility">Device compatibilty chart</a></li>
* <a href="https://github.com/mattharrison/epub-css-starter-kit">ePub CSS Starter Kit</a></li>
* <a href="http://code.google.com/p/epubcheck">ePub Validator</a></li>
* <a href="http://www.famkruithof.net/uuid/uuidgen">UUID generator</a></li>
* <a href="http://www.bisg.org/what-we-do-0-136-bisac-subject-headings-list-major-subjects.php">BISAC Subject Headings List</a></li>
* <a href="http://blog.threepress.org/2009/11/27/practical-epub-metadata-authorship/">Practical ePub metadata: Authorship</a></li>
* <a href="http://www.loc.gov/marc/relators">MARC Code List for Relators</a></li>

