# sth

## block site
```
geosite:category-ads-all,
clients2.googleusercontent.com,
update.googleapis.com,
clients1.google.com,
clients2.google.com
```

## surfingkeys 0.9.74 settings
```
// 更改bing.com网站
addSearchAliasX('b', 'bing', 'https://cn.bing.com/search?q=', 's', 'http://api.bing.com/osjson.aspx?query=', function(response) {
    var res = JSON.parse(response.text);
    return res[1];
});
// 用deepl翻译
addSearchAliasX('l', 'DeepL', 'https://www.deepl.com/zh/translator#en/zh/');
mapkey('ol', '#8Open Search with alias g', function() {
    Front.openOmnibar({type: "SearchEngine", extra: "l"});
});

settings.interceptedErrors = ["*"]; //错误页依然可以使用Surfingkeys，*代表所有页面
settings.tabsMRUOrder = false; // 按照顺序排列标签页
settings.tabsThreshold = 8; // 超过8个tab便改为列表显示
// 关于“0”与“$”
map('gxl', 'gxT');
map('gxh', 'gxt');
map('w', 'cS');



// set theme
settings.theme = `
.sk_theme {
    font-family: Input Sans Condensed, Charcoal, sans-serif;
    font-size: 9pt;
    background: #282828;
    color: #ebdbb2;
}
.sk_theme tbody {
    color: #b8bb26;
}
.sk_theme input {
    color: #d9dce0;
}
.sk_theme .url {
    color: #98971a;
}
.sk_theme .annotation {
    color: #b16286;
}
.sk_theme .omnibar_highlight {
    color: #eb5959;
}
.sk_theme #sk_omnibarSearchResult ul li:nth-child(odd) {
    background: #282828;
}
.sk_theme #sk_omnibarSearchResult ul li.focused {
    background: #26349e;
}
#sk_status, #sk_find {
    font-size: 9pt;
}`;
```


