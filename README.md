# TextformatterCodeBlocks

ProcessWire Textformatter module for enabling Markdown style code blocks for text or RTE fields.

Note: this is not a complete Markdown implementation, but rather a home-baked implementation of just one small part of the Markdown syntax. For full Markdown support, check out the TextformatterMarkdownExtra module, bundled with ProcessWire releases by default.

## Getting started

- Copy (or clone) the TextformatterCodeBlocks directory to /site/modules/
- Go to Admin > Modules, hit "Refresh", and install TextformatterCodeBlocks
- Enable "Code Blocks Textformatter" for fields in which you wish to use code blocks

IMPORTANT: if you use Code Blocks Textformatter with a regular text or textarea field, make sure that you enable HTML Entity Encoder or use another method of escaping entities!

## Code blocks

Code blocks should work fine when wrapped in <p> or <pre> tags, so you can use them with RTE, such as CKEditor. This module supports two types of code blocks: fenced and inline.

### Fenced code blocks

Simple example:

```
<?php
echo "This is a fenced code block.";
```

With fenced code blocks you can also specify the language for a syntax highlighter:

```php
<?php
echo "This PHP code is easier for a syntax highlighter to identify.";
```

The end result of fenced code blocks looks like this:

<pre class="code-block code-block--fenced"><code class="language-php">&lt;?php
echo "This PHP code is easier for a syntax highlighter to identify.";</code></pre>

### Inline code blocks

<p>While fenced code blocks are great for longer code snippets, sometimes `<?php echo "inline code blocks"; ?>` make more sense.</p>

The end result of inline code blocks looks like this:

<p>While fenced code blocks are great for longer code snippets, sometimes <code class="code-block code-block--inline">&lt;?php echo "inline code blocks"; ?&gt;</code> make more sense.</p>

## Enabling syntax highlighter

Though syntax highlighting is not necessary for this module to work, it can be really helpful for your end users. You can use any syntax highlighter, but I would recommend Prism.js.

For detailed instructions on enabling Prism.js on your site, please visit http://prismjs.com/.
