# Icons

Icons can be displayed in Stadium 6 by adding some simple CSS to the application StyleSheet. 

## Steps

1. Check the *Enable Style Sheet* checkbox in the application properties
2. Add a class to the control (e.g. `my-icon`)
3. Identify the element that contains the icon inside the rendered control (e.g. a `<button>` or `<a>` element). This requires you to inspect the control in the browser developer tools
4. Add a selector to the StyleSheet to target the icon element. For example, if the icon is inside a `<button>` element, you would use `.my-icon button`
6. Find the icon you want to use in the [Icones](https://icones.js.org/) library. Adjust the icon colour to the one matching your theme and copy the "Data Url" of the icon.
5. Add the following CSS to the StyleSheet:
```CSS
background-repeat: no-repeat;
background-size: <height and width of the icon>;
background-image: url("<the DATA URL for the icon>");
background-position: <position of the icon in the button>;
```

## Notes

1. Since this method displays the icon as a background image, the image size will not affect the width of height of the control. Add height and width attributes to the control if necessary. 
2. To place an icon next to text, add some padding to the control. For example, if the icon is on the left side of the text, you can add `padding-left: 30px;` to the control.