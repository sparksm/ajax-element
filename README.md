# &lt;ajax-element&gt;

> VanillaJS Ajax Web Component

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

3. Listen for Events:

    ```html
    <script>
      document.getElementById('myID').addEventListener('ajaxElementSuccess', function (event) {
        document.getElementById('anotherID').textContent = event.detail.data;
      });

      document.getElementById('myID').addEventListener('ajaxElementError', function (event) {
        document.getElementById('anotherID').textContent = event.detail.data;
      });
    </script>
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
