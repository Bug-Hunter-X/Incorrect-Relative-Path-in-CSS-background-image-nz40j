# Incorrect Relative Path in CSS background-image

This repository demonstrates a common issue encountered when using relative paths for background images in CSS. The problem arises when the CSS file and the image file are not located in the same directory, leading to the image failing to load.

## Bug Description
The provided CSS uses a relative path (`./image.png`) for the background image. However, if the image is not in the same directory as the CSS file, this path will be incorrect.

## Solution
The solution involves updating the relative path in the CSS to correctly point to the location of the `image.png` file. To ensure broader compatibility, it's recommended to use absolute paths or paths relative to the HTML file.

## How to Reproduce
1. Clone this repository.
2. Place `image.png` in a directory different from `bug.css`.
3. Open `index.html` in a web browser. You will notice that the background image does not load.
4. Replace `bug.css` with `solution.css` and refresh the page. The background image should now load successfully.