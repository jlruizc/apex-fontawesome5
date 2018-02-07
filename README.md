# Using Font Awesome 5 Pro in APEX

Blog: https://vmorneau.me/fontawesome5/  
Demo 1 (Custom): https://apex.oracle.com/pls/apex/f?p=114996  
Demo 2 (UT Demo): https://apex.oracle.com/pls/apex/f?p=114996  

**The following steps are required because of the Font Awesome 5 Pro license.**

I can't redistribute Font Awesome 5 Pro here, so you will have to download the files yourself and follow these steps:

### Download Steps
1. Get a license for Font Awesome 5 Pro: https://fontawesome.com/pro
3. Download APEX Font Awesome 5 compatibility files: https://github.com/vincentmorneau/apex-fontawesome5/tree/master/dist
3. Unzip Font Awesome 5 into `/dist/lib/fontawesome5`
4. Zip the whole `dist` folder
5. Upload it to your APEX web server
	- Example: Shared Components - Application Static Files: `#APP_IMAGES#`

### Option 1) SVG with JavaScript
1. Reference these JavaScript files in your app
	- `#APP_IMAGES#js/apex-fontawesome5#MIN#.js`
	- `#APP_IMAGES#lib/fontawesome5/svg-with-js/js/fontawesome-all#MIN#.js`
	- `#APP_IMAGES#lib/fontawesome5/svg-with-js/js/fa-v4-shims#MIN#.js`
2. Reference this CSS file in your app
	- `#APP_IMAGES#css/apex-fontawesome5#MIN#.css`
	
![](/doc/file-references-svg.png)
	
*Note: If your app shows flashing question marks as icons, it means that the icon you are using does not exist in Font Awesome 5.*

![](/doc/broken-icons.png)

### Option 2) Web Fonts with CSS
1. Reference this JavaScript file in your app
	- `#APP_IMAGES#js/apex-fontawesome5#MIN#.js`
2. Reference these CSS files in your app
	- `#APP_IMAGES#css/apex-fontawesome5#MIN#.css`
	- `#APP_IMAGES#lib/fontawesome5/web-fonts-with-css/css/fontawesome-all#MIN#.css`
	
![](/doc/file-references-css.png)

### Usage

##### Basic Usage
Pick your icon here https://fontawesome.com/icons.  
Use it in the appropriate icon CSS classes in APEX.

![](/doc/icon-css-classes-basic.png)

##### Styles & Prefixes
Style | Class
--- | ---
Solid | `fas`
Regular | `far`
Light | `fal`
Brand | `fab`

![](/doc/icon-css-classes-style.png)

##### Icon Sizes
Size | Class
--- | ---
0.75em | `fa-xs`
0.875em | `fa-sm`
1.33em | `fa-lg`
2em through 10em | `fa-2x` through `fa-10x`

![](/doc/icon-css-classes-size.png)

##### Animated
Animation | Class
--- | ---
Spin | `fa-spin`
Pulse | `fa-pulse`

![](/doc/icon-css-classes-spin.png)