# ToggleJS ✨
ToggleJS is a highly customizable toggle component, inspired by iOS-style switches. Crafted with pure JavaScript, this lightweight toggle offers an effortless integration into any web project. It stands out for its customization options and dynamic user interaction events, requiring no external dependencies.

## Features

- **Customizable**: Enables setting the toggle's color to match your project's design aesthetics.
- **Easy Integration**: Designed to be used as a directive within an HTML tag, making it straightforward to embed.
- **User Interaction Events**: Supports custom callback functions for interactive user engagements.
- **Dependency-Free**: Built with pure JavaScript, eliminating the need for any additional libraries.

## Installation

To incorporate ToggleJS into your project, simply copy the `ToggleJS` class code into a JavaScript file, for instance, `togglejs.js`.

## How to Use

Incorporating `ToggleJS` into your project is easy. Follow these steps for a quick setup:

### 1. Add the HTML Element

Place a `toggle-js` element in your HTML file where you want the toggle to appear.

```html
<toggle-js id="myToggle"></toggle-js>
```
### 2\. Initialize ToggleJS

Include the `togglejs.js` file in your project and initialize `ToggleJS` by passing the element selector and an options object.

```html

<script src="path/to/togglejs.js"></script>
<script> // Function to call when the toggle state changes
  function myPersonalMethod(checked) {
    console.log('Toggle is now:', checked ? 'ON' : 'OFF');
  }

  // Initialize ToggleJS
  new ToggleJS('#myToggle', {
    color: '#F00000', // Custom toggle color
    onclick: myPersonalMethod // Callback to handle state changes
  }); </script>
```

### Options

When initializing `ToggleJS`, you can pass an options object to customize the toggle's behavior:

-   color: Sets the toggle's color. Default is `#ccc`.
-   onclick: A callback function that gets called whenever the toggle's state changes. The function receives a `checked` argument, which is `true` if the toggle is on, and `false` otherwise.

### Events

`ToggleJS` triggers a custom `toggleChange` event every time the toggle's state changes. You can listen to this event on the `toggle-js` element to execute custom logic:

```javascript

document.querySelector('#myToggle').addEventListener('toggleChange', function(e) {
  console.log('Toggle changed:', e.detail.checked ? 'ON' : 'OFF');
});
```

Contributing
------------

Contributions to the project are welcome. To contribute, please fork the repository, create a feature or bugfix branch, and submit a pull request.

License
-------

ToggleJS is distributed under the MIT License.


Frequently Asked Questions (FAQs)
-------

### What is ToggleJS?

ToggleJS is a lightweight, pure JavaScript component for creating customizable toggle switches. It offers a simple way to integrate iOS-style toggles into any web project, enhancing UI interactivity with minimal effort.

### How do I customize the color of a ToggleJS switch?

Customizing your toggle's color with ToggleJS is straightforward. When initializing the ToggleJS component, pass a color option to set your desired toggle color, ensuring your toggle css aligns perfectly with your project's design.

### Can ToggleJS be used in any web project?

Yes, ToggleJS is designed for universal compatibility. Its dependency-free, pure JavaScript implementation makes it a versatile choice for any web project, from simple blogs to complex web applications.

### Is ToggleJS easy to integrate with HTML?

Absolutely! ToggleJS is built to be easily integrated into your HTML with a simple directive. Just add a `toggle-js` tag where you want the toggle to appear, and initialize ToggleJS in your JavaScript file. This approach makes adding a "simple toggle js" to your project effortless.

### How can I handle toggle events with ToggleJS?

ToggleJS supports custom callback functions through its `onclick` option. This feature allows you to execute any JavaScript code when the toggle changes state, providing a dynamic way to respond to user interactions.

### Does ToggleJS support TypeScript?

While ToggleJS is primarily written in pure JavaScript, it can be easily adapted to support TypeScript projects. Including basic type definitions for the options and events can enhance your development experience with type safety.

### How does ToggleJS improve web project accessibility?

ToggleJS toggles are designed with accessibility in mind. By following best practices for interactive components, including keyboard navigability and ARIA attributes, ToggleJS helps ensure your web projects are accessible to all users.

### Where can I find documentation for ToggleJS?

Comprehensive documentation for ToggleJS, including installation instructions, usage examples, and customization options, is available on the official ToggleJS GitHub repository. This resource provides everything you need to get started with "toggle js" in your projects.

### How can I contribute to ToggleJS?

Contributions to ToggleJS are welcomed and appreciated. Whether you're fixing a bug, adding a feature, or improving documentation, you can contribute by forking the repository, making your changes, and submitting a pull request.
