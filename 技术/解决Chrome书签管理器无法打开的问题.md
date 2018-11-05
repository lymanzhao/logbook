1 出现的问题

谷歌浏览器Chrome的扩展程序[书签管理器（Bookmark Manager）](https://chrome.google.com/webstore/detail/bookmark-manager/gmlllbghnfkpflemihljekbapjopfjik)在Chrome某次版本升级后就打不开了。具体情况是，点击Chrome状态栏右侧“三个竖点” > “书签（Bookmarks）” > “书签管理器（Bookmark manager）”，会出现如下提示：

eemcgdkfndhakfknompkggombfjjjeno is blocked  Requests to the server have been blocked by an extension.  Try disabling your extensions.  ERR_BLOCKED_BY_CLIENT

eemcgdkfndhakfknompkggombfjjjeno 已被屏蔽  对服务器的请求已遭到某个扩展程序的阻止。  尝试停用扩展程序。  ERR_BLOCKED_BY_CLIENT

2 解决的方法

在地址栏中输入：

chrome://flags/#enable-md-bookmarks

将默认的“Default”改为“Disabled”，重启浏览器，问题解决。

原因是[Material Design书签功能目前存在bug](https://productforums.google.com/forum/#!msg/chrome/7uyLxeEI5aw/J8nAX8yOBgAJ)，关闭就好了。