# Svelte Custom Card

![](https://img.shields.io/github/license/1mpossible-code/svelte-custom-card?color=green)

Customizable and minimalistic svelte Card component.

* [Description](#description)
* [Installation](#installation)
* [Usage](#usage)
* [Contributing](#contributing)
* [Credits](#credits)
* [License](#license)

----

## Description

Svelte Custom Card is a project that implements the most simple, flexible, customizable, light and minimalistic card
component with [Svelte](https://svelte.dev/).

## Installation

* To use [Card](https://github.com/1mpossible-code/svelte-custom-card/blob/master/src/Card.svelte) in your component
  just download it with cURL, wget or just copy
  [raw](https://raw.githubusercontent.com/1mpossible-code/svelte-custom-card/master/src/Card.svelte) from the browser.

```bash
# cURL
curl -o https://raw.githubusercontent.com/1mpossible-code/svelte-custom-card/master/src/Card.svelte
# wget
wget https://raw.githubusercontent.com/1mpossible-code/svelte-custom-card/master/src/Card.svelte
```

* To test Card component do following:

```bash
git clone https://github.com/1mpossible-code/svelte-custom-card.git
cd svelte-custom-card
npm install
npm run dev
```

## Usage

To use this Card you need to import it to your svelte component. Then there are 2 ways to specify data to it. Card has 2
default slots: `title` and `description`.

To add image to the card use prop `image` where you need to specify the link to your image.

To make a link you may use default button (specify props `link` and `linkTitle` with the url and title accordingly) or
slot `link` with your own designed button.

[Example of real usage.](src/App.svelte)

### Example usage

```svelte
<script>
    import Card from './Card.svelte'
</script>

<div>
      <!-- Card with prop link -->
      <Card image="https://via.placeholder.com/320x180/" link="https://example.com" linkTitle="Link">
          <h3 slot="title">Title</h3>
          <p slot="description">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Commodi, ratione!</p>
      </Card>
      
      <!-- Card with slot link -->
      <Card image="https://via.placeholder.com/320x180/">
          <h3 slot="title">Title 2</h3>
          <p slot="description">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Commodi, ratione!</p>
          <a slot="link" href="https://example.com">Link</a>
      </Card>
</div>
```

## Contributing

Feel freely to contribute this project. [Issues](https://github.com/1mpossible-code/svelte-custom-card/issues)
and [PRs](https://github.com/1mpossible-code/svelte-custom-card/pulls) are welcome!

## Credits

You can mail to `linme00p@gmail.com` to contact the author

# License

Copyright © 2021 [1mpossible-code](https://github.com/1mpossible-code). This project
is [GPLv3](https://www.https://www.gnu.org/licenses/gpl-3.0.htmlgnu.org/licenses/gpl-3.0) licensed.
