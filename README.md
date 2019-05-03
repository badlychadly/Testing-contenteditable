# Testing-contenteditable

This is just a short reading of something I came across recently and wanted to implement in my own code. I have been very curious about how a blogging platform works lately. I'm talking about all of these sites that have a cool toolbar that can be used to add as many headings, links, and block quotes as a user wants. I am no expert here, but I did finally come across something on a site I was inspecting the html of and that is `contenteditable`.

### Contenteditable
`contenteditable` is an html attribute that specifies if an elements content is editable or not. This is cool because instead of using an `input` tag I can use other elements such as `a`, `h1`, and `p` inside a parent element that I have given the `contenteditable` attribute to. This seems like the doorway I have been looking for to enable client side editing on my blogging app. Also once you set `contenteditable` to true you get access to the `document.execCommand()`, which allows you to run commands to manipulate the contents of the editable region.


### ExecCommand()
Using the `execCommand()` you can make changes based on the current selection. This can come in handy with event like focus and blur. `execCommand()` take three arguments `aCommandName`, `aShowDefaultUI`, and `aValueArgument`. There is a list of commands you can check out in the [documentation](https://developer.mozilla.org/en-US/docs/Web/API/Document/execCommand).

This is just my basic understanding of using `contenteditable` and I have much I still need to find out. I also need to figure out how to use this in React without causing issues, but I will keep at it and figure it out!
