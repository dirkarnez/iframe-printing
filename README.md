[iframe-printing](https://dirkarnez.github.io/iframe-printing)
==============================================================
### Notes
- ```css
  @media print { @page { size: A4; } }
  ```
- ```js
  const element = document.getElementById('print-container');
  const isOverflowing = element.scrollHeight > element.clientHeight;
  ```
- ```js
      doc = iframe.contentWindow.document;
      // 引入打印的专有CSS样式，根据实际修改
      doc.write(`<head><style type="text/css">${styleTem}</style></head>`);
      doc.write('<div>' + el.innerHTML + '</div>');
      doc.close();
      iframe.contentWindow.focus();
      iframe.contentWindow.print();
  ```
