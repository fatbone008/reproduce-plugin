# demo

## Testing lib

run ```npm install path/to/lib```, install testing lib by file mode through npm

The "lib" is the one export a button with setup() including a injected variable.

and import it in HelloWorld.vue as an component.

Here the issue is, in the imported component, the variable "sarah" in setup is undefined if checked in the devtool.

But when I create a identical component(MyTesting.vue) in this project. The variable "sarah" possess the provided value.
