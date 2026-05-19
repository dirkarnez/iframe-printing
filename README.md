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
