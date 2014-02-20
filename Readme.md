*This repository is a mirror of the [component](http://component.io) module [jasonkuhrt/force-redraw](http://github.com/jasonkuhrt/force-redraw). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/jasonkuhrt-force-redraw`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# force-redraw
  Force the browser to repaint an element

## Installation
  Install with [component(1)](http://component.io):
    $ component install jasonkuhrt/force-redraw

## API
    force_redraw()
  Refresh the `document.body` element. Typically you won't want to do this because it may well result in a blink-like flicker of the user-interface.

    force_redraw(dom_element)
  Redraw the given DOM element.

## Notes
  This function's usefulness is particularly relevant for webkit where buggy css rendering issues have cropped up in my client-side apps. Others have encountered this problem too:
  http://stackoverflow.com/questions/3485365/how-can-i-force-webkit-to-redraw-repaint-to-propagate-style-changes.

## License
  BSD-2-Clause