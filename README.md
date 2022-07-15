# What is this?

This is randomColor for change background

# Installation

`npm install hex_btn-2`

# Using...
```
import { renderHexes } from "nex_btn-2";
function renderHexes() {
  let temp = "0123456789ABCDEF";
  let color = "#";
  for (let i = 0; i < 6; i++) {
    color += temp[Math.floor(Math.random() * 16)];
  }
  return color;
}

allBtn.forEach((index) => {
  let color = renderHexes();
  index.style.backgroundColor = color;
  index.innerHTML = color;
  index.addEventListener("click", () => {
    document.body.style.backgroundColor = color;
  });
});
```