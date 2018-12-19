# jsoup_practice

# 按照超链接文字得到超链接

Elements links = doc.getElementsByTag("a");
for (Element link : links) {

  String linkText = link.text();
  if (linkText.contains("Next page")) {
    String linkHref = link.attr("href");
    urlstr = linkHref;
    break;
  }
}
  
