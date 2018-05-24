# Storybook + Vue Hack Session
## About Storybook
Storybook for Vue is a UI development environment for UI components. It allows interactive development, testing and sharing of UI components in various property states.

Storybook runs outside of your app. So you can develop UI components in isolation without worrying about app specific dependencies and requirements.

## Getting Started
```bash
git clone https://github.com/micahscopes/storybook-vue-hack-session.git
cd storybook-vue-hack-session
```
## Storybook Setup

```bash
# run storybook
yarn install
yarn run storybook
```
Storybook should now be running at [http://localhost:9001/
](http://localhost:9001/).

Stories are referenced in [./src/stories/index.js](./src/stories/index.js).
## Using Storybook with Vue
Much of the documentation for Storybook is written with React in mind, you can check this document for information on how to use Storybook with Vue:
- [Storybook for Vue / Write your stories](https://storybook.js.org/basics/guide-vue/#write-your-stories).

## Stuff to try
- #### Make a simple story
    The [vuetify component library](https://github.com/vuetifyjs/vuetify) is already included.  You can use them to make a simple story.  For example:
```javascript
storiesOf("VBtn", module).add("it's a button!", () => ({
  template: `
  <v-app>
    <v-btn>a button!</v-btn>
  </v-app>
  `
}));
```
- #### Import a custom component and use it in a story
    You can use the examples in [./src/stories/index.js](./src/stories/index.js) as a reference.

- #### Build a multi-part story
    By chaining together `add` functions, you can make stories with multiple parts.

- #### Do something elaborate, yet basic
    Check out [this guide](https://storybook.js.org/basics/writing-stories/) for ideas of fancy things to try.  Examples include nested stories,  

- #### Addons: truely elaborate
    Storybook can be used [with addons](https://storybook.js.org/addons/introduction/).  Check the [Addon Gallery](https://storybook.js.org/addons/addon-gallery/) for inspiration.

- #### Try it with Jest
    There is a [Jest addon](https://github.com/storybooks/storybook-addon-jest).  Can you get it working?

- #### Write an essay
    Maybe you have some ideas on how this tool could be applied in real life.  Write your ideas down in an essay!

## Using this as a boilerplate
You can also use this as a Vuetify+Storybook boilerplate:

```bash
# serve with hot reload at localhost:8080
yarn run dev

# build for production with minification
yarn run build
```

## Credits
> This boilerplate was forked from [White Rabbit Express](https://github.com/white-rabbit-japan/vuetify-storyboard-boilerplate)
