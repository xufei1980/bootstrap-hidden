# bootstrap-hidden
BootStrap 不同隐藏方式
使用 Bootstrap 4 顯示/隱藏 HTML 元素
https://poychang.github.io/visible-and-hidden-in-bootstrap-4/

AUGUST 25TH, 2017
Bootstrap 千呼萬喚來到了 v4 beta，裡面除了提供更好看的元件外，以提供了許多好用個工具，讓排版變得更輕鬆，這對 CSS 苦手的我，真是一大福音，但是使用的時候發現一個問題，前幾版都有的 visible 和 hidden 類別好像變得不容易用了…

在 Bootstrap 3 的時候，有 Responsive Utilities 讓我們控制響應式顯示，可以參考下表來設定。

Bootstrap 3 - Responsive Utilities 

很方便對吧！

到了 Bootstrap 4-alpha 的時候，改成用 Display Property 來做控制，而 Bootstrap 4 Beta 也依照這樣的方式繼續走下去。

這樣做也不會說不好，保留了更多彈性去使用，只是對我這位 CSS 苦手來說有一點不直覺，所以整理了最下面的表格，方便我之後使用。

Display 通用類別
Display 通用類別，可用於切換元件的顯示與否，並且可以包含響應式設定，基本的變化如下：

CSS Class	說明
d-none	不顯示也不佔空間
d-inline	行內並排容器，大小以內容物判定
d-inline-block	行內塊狀容器，大小以內容物判定，可設定寬高、上下外距等屬性
d-block	塊狀容器，大小以空間判定，可設定寬高、上下外距等屬性
d-table	表格容器
d-table-cell	表格元素容器
d-flex	塊級伸縮容器
d-inline-flex	行內級伸縮容器
搭配響應式的類型做變化
有了 Display 通用類別，再搭配響應式的設定，就可以做出響應式顯示/隱藏 HTML 元素的功能。

BS 3	BS 4	備註
hidden-xs-down	d-none d-sm-block	
hidden-sm-down	d-none d-md-block	
hidden-md-down	d-none d-lg-block	
hidden-lg-down	d-none d-xl-block	
hidden-xl-down	d-none	(same as hidden)
hidden-xs-up	d-none	(same as hidden)
hidden-sm-up	d-sm-none	
hidden-md-up	d-md-none	
hidden-lg-up	d-lg-none	
hidden-xl-up	d-xl-none	
hidden-xs	d-none d-sm-block	(only)
hidden-sm	d-block d-sm-none d-md-block	(only)
hidden-md	d-block d-md-none d-lg-block	(only)
hidden-lg	d-block d-lg-none d-xl-block	(only)
hidden-xl	d-block d-xl-none	(only)
visible-xs	d-block d-sm-none	(only)
visible-sm	d-none d-sm-block d-md-none	(only)
visible-md	d-none d-md-block d-lg-none	(only)
visible-lg	d-none d-lg-block d-xl-none	(only)
visible-xl	d-none d-xl-block	(only)
整理完後，仿造原本的表格樣式做一個對照表。



參考資料：

Bootstrap - Visibility
Missing visible-** and hidden-** in Bootstrap v4
Bootstrap 4 Hidden & Visible
CSS 基本Display屬性
