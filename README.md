# JSON5 Editor: IDE-like Editor to Prettify / Minify / Verify JSON
[JSON5 Editor](https://json-5.com) is a user-friendly JSON editor that facilitates the editing of both JSON and JSON5. However, JSON5 has more flexible syntax by allowing omitting quotes around keys, multi-line commenting, and trailing commas in arrays and objects. This makes JSON editing process more efficient and productive.

Moreover, [JSON5 Editor](https://json-5.com) is a text editor similar to VS code, allowing users to work on multiple tabbed files simultaneously, rename tabs, drag and drop tabs, and use other [VS code editing techniques](https://code.visualstudio.com/docs/editor/codebasics) such as selecting all occurrences of a selected word. It helps you keep work organized and increases productivity.

Key features:
- Error-free JSON editing experience.
- Key bindings and shortcuts are compatible with Visual Studio Code.
- High performance parsing and formartting JSON Data.
- Integration with Alfred to boost productivity.

## Use JSON5 Edtior for free now: https://json-5.com

![JSON-5](https://user-images.githubusercontent.com/3455798/226092084-5977ae57-b643-473a-a0bd-b937084b07f7.gif)

## 1. Error-free JSON editing experience.

### 1.1 Comma
- Arrays having a single trailing comma are allowed.
- Objects having a single trailing comma are allowed.
- Missing comma in object is allowed.

```js
{
  "key1": [1, 2, ], // Trailing comma in array
  "key2": { "key1": "string", },  // Trailing comma in object 
  "key3": "string" // --> Missing comma in object is allowed
  "key4": "string"
}
```
![image](https://user-images.githubusercontent.com/3455798/226093599-ca5e8319-75fd-4c5d-861d-3ef0e0a53490.png)


### 1.2 Comment
- Single comment(// or #) is allowed.
- Multi-line comment(/* */) is allowed.


```js
{
  // "key1": "string",

  /* "key2": "string",
     "key3": "string", */

  #  "key4": "string",
}
```
![image](https://user-images.githubusercontent.com/3455798/226093818-36c2cd20-0b35-4384-9ff1-7b3c3752ae40.png)


### 1.3 String
- Single quoted string is allowd.

```js
{
  singleQuotes: 'Use "double quotes"',
}
```
![image](https://user-images.githubusercontent.com/3455798/226093775-ce2e1a7c-cc47-43a9-9498-614e036c4492.png)


### 1.4 Object key

- keys could be an ECMAScript 5.1 [IdentifierName](https://262.ecma-international.org/5.1/#sec-7.6).
- keys without quotes are allowed.
```js
{
  "$string": "string", // ECMAScript 5.1 IdentifierName
  unquoted: 'string' // Key without quotes
}
```
![image](https://user-images.githubusercontent.com/3455798/226093494-66983740-9a00-4041-bdc1-613732e89253.png)

## 2. Editor shortcuts
Key bindings are fully compatible with [Visual Studio Code](https://code.visualstudio.com/docs/editor/codebasics). Here are some useful tips.

### 2.1 Multiple selections
`⌘D` selects the word at the cursor, or the next occurrence of the current selection.

<img style="width:400px" src="https://user-images.githubusercontent.com/3455798/226115913-658541ea-3b5f-448d-b83a-b08459a3a492.png" />

### 2.2 Folding / unfolding left pane
`⌘B` folds / unfolds left pane quickly.

<img style="width:400px" src="https://user-images.githubusercontent.com/3455798/226117055-9ae01abf-a72a-4e25-beec-7e7346883eb2.png" />


### 3. Integration with Alfred
As a software developer, you can easily open your JSON data in the editor via Alfred's customizable web searches. This integration allows you to format your JSON data quickly and efficiently.

You can use it by typing "json" followed by your JSON data in [Alfred](https://www.alfredapp.com). For example:
![Alfred json](https://user-images.githubusercontent.com/3455798/229289708-0398eb8f-4017-455a-a8bf-950256c32feb.png)

This will open the JSON5 editor in your browser with the provided data already loaded.

![Alfred json](https://user-images.githubusercontent.com/3455798/229290034-62e3d6dc-e35d-4094-88b9-15ea44323ffe.png)

To add this JSON editor [custom search](https://www.alfredapp.com/help/features/web-search/custom-searches) to [Alfred](https://www.alfredapp.com), simply enter the following command in your browser's URL bar. A pop-up will appear asking if you want to import the custom search.

```
alfred://customsearch/json%20format/json/utf8/nospace/https://json-5.com/#inputText=%7Bquery%7D
```


## 4. Data Privacy
We can assure you that your input data in [json-5.com](json-5.com) is stored securely in your browser's [localStorage](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage) only, which is not shared with any third-party, ensuring complete privacy and confidentiality.
