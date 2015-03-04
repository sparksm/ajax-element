# &lt;ajax-element&gt;

> ajax web component

## Demo

[Check it live!](http://sparksm.github.io/ajax-element)

## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install ajax-element --save
```

Or [download as ZIP](https://github.com/sparksm/ajax-element/archive/master.zip).

## Usage

1. Import Web Components' polyfill:

    ```html
    <script src="bower_components/webcomponentsjs/webcomponents.min.js"></script>
    ```

2. Import Custom Element:

    ```html
    <link rel="import" href="bower_components/ajax-element/src/ajax-element.html">
    ```

3. Start using it!

    ```html
    <ajax-element src="http://www.example.com"></ajax-element>
    ```

## Options

Attribute     | Options     | Default      | Description
---           | ---         | ---          | ---
`url`         | *string*    | ``           | The Request URL.
`type`        | *string*    | `GET`        | The Request Method.
`datatype`    | *string*    | ``           | Set to `json` to parse response as JSON.
`data`        | *string*    | ``           | Set to serialized data to send with POST requests.

## Methods

Method        | Parameters   | Returns     | Description
---           | ---          | ---         | ---
`unicorn()`   | None.        | Nothing.    | Magic stuff appears.

## Events

Event         | Description
---           | ---
`onsomething` | Triggers when something happens.

## Development

In order to run it locally you'll need to fetch some dependencies and a basic server setup.

* Install [Bower](http://bower.io/) & [Grunt](http://gruntjs.com/):

    ```sh
    $ [sudo] npm install -g bower grunt-cli
    ```

* Install local dependencies:

    ```sh
    $ bower install && npm install
    ```

* To test your project, start the development server and open `http://localhost:8000`.

    ```sh
    $ grunt server
    ```

* To provide a live demo, send everything to `gh-pages` branch.

    ```sh
    $ grunt deploy
    ```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## History

For detailed changelog, check [Releases](https://github.com/sparksm/ajax-element/releases).

## License

[MIT License](http://opensource.org/licenses/MIT)
