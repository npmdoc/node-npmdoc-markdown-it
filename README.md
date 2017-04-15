# api documentation for  [markdown-it (v8.3.1)](https://github.com/markdown-it/markdown-it#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-markdown-it.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-markdown-it) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-markdown-it.svg)](https://travis-ci.org/npmdoc/node-npmdoc-markdown-it)
#### Markdown-it - modern pluggable markdown parser.

[![NPM](https://nodei.co/npm/markdown-it.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/markdown-it)

[![apidoc](https://npmdoc.github.io/node-npmdoc-markdown-it/build/screenCapture.buildCi.browser.apidoc.html.png)](https://npmdoc.github.io/node-npmdoc-markdown-it/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-markdown-it/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-markdown-it/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bin": {
        "markdown-it": "bin/markdown-it.js"
    },
    "bugs": {
        "url": "https://github.com/markdown-it/markdown-it/issues"
    },
    "dependencies": {
        "argparse": "^1.0.7",
        "entities": "~1.1.1",
        "linkify-it": "^2.0.0",
        "mdurl": "^1.0.1",
        "uc.micro": "^1.0.3"
    },
    "description": "Markdown-it - modern pluggable markdown parser.",
    "devDependencies": {
        "ansi": "^0.3.0",
        "autoprefixer-stylus": "^0.11.0",
        "benchmark": "~2.1.0",
        "browserify": "*",
        "chai": "^3.4.1",
        "coveralls": "~2.11.9",
        "eslint": "^3.5.0",
        "express": "^4.14.0",
        "highlight.js": "^9.2.0",
        "istanbul": "^0.4.5",
        "jade": "~1.11.0",
        "markdown-it-abbr": "^1.0.4",
        "markdown-it-container": "^2.0.0",
        "markdown-it-deflist": "^2.0.0",
        "markdown-it-emoji": "^1.1.1",
        "markdown-it-footnote": "^3.0.1",
        "markdown-it-for-inline": "~0.1.0",
        "markdown-it-ins": "^2.0.0",
        "markdown-it-mark": "^2.0.0",
        "markdown-it-sub": "^1.0.0",
        "markdown-it-sup": "^1.0.0",
        "markdown-it-testgen": "~0.1.3",
        "mocha": "*",
        "ndoc": "^5.0.0",
        "stylus": "~0.54.2",
        "uglify-js": "^2.7.3"
    },
    "directories": {},
    "dist": {
        "shasum": "2f4b622948ccdc193d66f3ca2d43125ac4ac7323",
        "tarball": "https://registry.npmjs.org/markdown-it/-/markdown-it-8.3.1.tgz"
    },
    "files": [
        "index.js",
        "bin/",
        "lib/",
        "dist/"
    ],
    "gitHead": "427cc20c9b9dd73b8e00b33f48cc643042261a1b",
    "homepage": "https://github.com/markdown-it/markdown-it#readme",
    "keywords": [
        "markdown",
        "parser",
        "commonmark",
        "markdown-it",
        "markdown-it-plugin"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "vitaly"
        }
    ],
    "name": "markdown-it",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/markdown-it/markdown-it.git"
    },
    "scripts": {
        "heroku-postbuild": "npm install express",
        "test": "make test"
    },
    "version": "8.3.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module markdown-it](#apidoc.module.markdown-it)
1.  [function <span class="apidocSignatureSpan"></span>markdown-it (presetName, options)](#apidoc.element.markdown-it.markdown-it)
1.  [function <span class="apidocSignatureSpan">markdown-it.</span>parser_block ()](#apidoc.element.markdown-it.parser_block)
1.  [function <span class="apidocSignatureSpan">markdown-it.</span>toString ()](#apidoc.element.markdown-it.toString)
1.  object <span class="apidocSignatureSpan">markdown-it.</span>parser_block.prototype

#### [module markdown-it.parser_block](#apidoc.module.markdown-it.parser_block)
1.  [function <span class="apidocSignatureSpan">markdown-it.</span>parser_block ()](#apidoc.element.markdown-it.parser_block.parser_block)

#### [module markdown-it.parser_block.prototype](#apidoc.module.markdown-it.parser_block.prototype)
1.  [function <span class="apidocSignatureSpan">markdown-it.parser_block.prototype.</span>State (src, md, env, tokens)](#apidoc.element.markdown-it.parser_block.prototype.State)
1.  [function <span class="apidocSignatureSpan">markdown-it.parser_block.prototype.</span>parse (src, md, env, outTokens)](#apidoc.element.markdown-it.parser_block.prototype.parse)
1.  [function <span class="apidocSignatureSpan">markdown-it.parser_block.prototype.</span>tokenize (state, startLine, endLine)](#apidoc.element.markdown-it.parser_block.prototype.tokenize)



# <a name="apidoc.module.markdown-it"></a>[module markdown-it](#apidoc.module.markdown-it)

#### <a name="apidoc.element.markdown-it.markdown-it"></a>[function <span class="apidocSignatureSpan"></span>markdown-it (presetName, options)](#apidoc.element.markdown-it.markdown-it)
- description and source-code
```javascript
function MarkdownIt(presetName, options) {
  if (!(this instanceof MarkdownIt)) {
    return new MarkdownIt(presetName, options);
  }

  if (!options) {
    if (!utils.isString(presetName)) {
      options = presetName || {};
      presetName = 'default';
    }
  }

<span class="apidocCodeCommentSpan">  /**
   * MarkdownIt#inline -> ParserInline
   *
   * Instance of [[ParserInline]]. You may need it to add new rules when
   * writing plugins. For simple rules control use [[MarkdownIt.disable]] and
   * [[MarkdownIt.enable]].
   **/
</span>  this.inline = new ParserInline();

  /**
   * MarkdownIt#block -> ParserBlock
   *
   * Instance of [[ParserBlock]]. You may need it to add new rules when
   * writing plugins. For simple rules control use [[MarkdownIt.disable]] and
   * [[MarkdownIt.enable]].
   **/
  this.block = new ParserBlock();

  /**
   * MarkdownIt#core -> Core
   *
   * Instance of [[Core]] chain executor. You may need it to add new rules when
   * writing plugins. For simple rules control use [[MarkdownIt.disable]] and
   * [[MarkdownIt.enable]].
   **/
  this.core = new ParserCore();

  /**
   * MarkdownIt#renderer -> Renderer
   *
   * Instance of [[Renderer]]. Use it to modify output look. Or to add rendering
   * rules for new token types, generated by plugins.
   *
   * ##### Example
   *
   * '''javascript
   * var md = require('markdown-it')();
   *
   * function myToken(tokens, idx, options, env, self) {
   *   //...
   *   return result;
   * };
   *
   * md.renderer.rules['my_token'] = myToken
   * '''
   *
   * See [[Renderer]] docs and [source code](https://github.com/markdown-it/markdown-it/blob/master/lib/renderer.js).
   **/
  this.renderer = new Renderer();

  /**
   * MarkdownIt#linkify -> LinkifyIt
   *
   * [linkify-it](https://github.com/markdown-it/linkify-it) instance.
   * Used by [linkify](https://github.com/markdown-it/markdown-it/blob/master/lib/rules_core/linkify.js)
   * rule.
   **/
  this.linkify = new LinkifyIt();

  /**
   * MarkdownIt#validateLink(url) -> Boolean
   *
   * Link validation function. CommonMark allows too much in links. By default
   * we disable 'javascript:', 'vbscript:', 'file:' schemas, and almost all 'data:...' schemas
   * except some embedded image types.
   *
   * You can change this behaviour:
   *
   * '''javascript
   * var md = require('markdown-it')();
   * // enable everything
   * md.validateLink = function () { return true; }
   * '''
   **/
  this.validateLink = validateLink;

  /**
   * MarkdownIt#normalizeLink(url) -> String
   *
   * Function used to encode link url to a machine-readable format,
   * which includes url-encoding, punycode, etc.
   **/
  this.normalizeLink = normalizeLink;

  /**
   * MarkdownIt#normalizeLinkText(url) -> String
   *
   * Function used to decode link url to a human-readable format'
   **/
  this.normalizeLinkText = normalizeLinkText;


  // Expose utils & helpers for easy acces from plugins

  /**
   * MarkdownIt#utils -> utils
   *
   * Assorted utility functions, useful to write plugins. See details
   * [here](https://github.com/markdown-it/markdown-it/blob/master/lib/common/utils.js).
   **/
  this.utils = utils;

  /**
   * MarkdownIt#helpers -> helpers
   *
   * Link components parser functions, useful to write plugins. See details
   * [here](https://github.com/markdown-it/markdown-it/blob/master/lib/helpers).
   **/
  this.helpers = utils.assign({}, helpers);


  this.options = {};
  this.configure(presetName);

  if (options) { this.set(options); }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.markdown-it.parser_block"></a>[function <span class="apidocSignatureSpan">markdown-it.</span>parser_block ()](#apidoc.element.markdown-it.parser_block)
- description and source-code
```javascript
function ParserBlock() {
<span class="apidocCodeCommentSpan">  /**
   * ParserBlock#ruler -> Ruler
   *
   * [[Ruler]] instance. Keep configuration of block rules.
   **/
</span>  this.ruler = new Ruler();

  for (var i = 0; i < _rules.length; i++) {
    this.ruler.push(_rules[i][0], _rules[i][1], { alt: (_rules[i][2] || []).slice() });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.markdown-it.toString"></a>[function <span class="apidocSignatureSpan">markdown-it.</span>toString ()](#apidoc.element.markdown-it.toString)
- description and source-code
```javascript
toString = function () {
    return toString;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.markdown-it.parser_block"></a>[module markdown-it.parser_block](#apidoc.module.markdown-it.parser_block)

#### <a name="apidoc.element.markdown-it.parser_block.parser_block"></a>[function <span class="apidocSignatureSpan">markdown-it.</span>parser_block ()](#apidoc.element.markdown-it.parser_block.parser_block)
- description and source-code
```javascript
function ParserBlock() {
<span class="apidocCodeCommentSpan">  /**
   * ParserBlock#ruler -> Ruler
   *
   * [[Ruler]] instance. Keep configuration of block rules.
   **/
</span>  this.ruler = new Ruler();

  for (var i = 0; i < _rules.length; i++) {
    this.ruler.push(_rules[i][0], _rules[i][1], { alt: (_rules[i][2] || []).slice() });
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.markdown-it.parser_block.prototype"></a>[module markdown-it.parser_block.prototype](#apidoc.module.markdown-it.parser_block.prototype)

#### <a name="apidoc.element.markdown-it.parser_block.prototype.State"></a>[function <span class="apidocSignatureSpan">markdown-it.parser_block.prototype.</span>State (src, md, env, tokens)](#apidoc.element.markdown-it.parser_block.prototype.State)
- description and source-code
```javascript
function StateBlock(src, md, env, tokens) {
  var ch, s, start, pos, len, indent, offset, indent_found;

  this.src = src;

  // link to parser instance
  this.md     = md;

  this.env = env;

  //
  // Internal state vartiables
  //

  this.tokens = tokens;

  this.bMarks = [];  // line begin offsets for fast jumps
  this.eMarks = [];  // line end offsets for fast jumps
  this.tShift = [];  // offsets of the first non-space characters (tabs not expanded)
  this.sCount = [];  // indents for each line (tabs expanded)

  // An amount of virtual spaces (tabs expanded) between beginning
  // of each line (bMarks) and real beginning of that line.
  //
  // It exists only as a hack because blockquotes override bMarks
  // losing information in the process.
  //
  // It's used only when expanding tabs, you can think about it as
  // an initial tab length, e.g. bsCount=21 applied to string '\t123'
  // means first tab should be expanded to 4-21%4 === 3 spaces.
  //
  this.bsCount = [];

  // block parser variables
  this.blkIndent  = 0; // required block content indent
                       // (for example, if we are in list)
  this.line       = 0; // line index in src
  this.lineMax    = 0; // lines count
  this.tight      = false;  // loose/tight mode for lists
  this.ddIndent   = -1; // indent of the current dd block (-1 if there isn't any)

  // can be 'blockquote', 'list', 'root', 'paragraph' or 'reference'
  // used in lists to determine if they interrupt a paragraph
  this.parentType = 'root';

  this.level = 0;

  // renderer
  this.result = '';

  // Create caches
  // Generate markers.
  s = this.src;
  indent_found = false;

  for (start = pos = indent = offset = 0, len = s.length; pos < len; pos++) {
    ch = s.charCodeAt(pos);

    if (!indent_found) {
      if (isSpace(ch)) {
        indent++;

        if (ch === 0x09) {
          offset += 4 - offset % 4;
        } else {
          offset++;
        }
        continue;
      } else {
        indent_found = true;
      }
    }

    if (ch === 0x0A || pos === len - 1) {
      if (ch !== 0x0A) { pos++; }
      this.bMarks.push(start);
      this.eMarks.push(pos);
      this.tShift.push(indent);
      this.sCount.push(offset);
      this.bsCount.push(0);

      indent_found = false;
      indent = 0;
      offset = 0;
      start = pos + 1;
    }
  }

  // Push fake entry to simplify cache bounds checks
  this.bMarks.push(s.length);
  this.eMarks.push(s.length);
  this.tShift.push(0);
  this.sCount.push(0);
  this.bsCount.push(0);

  this.lineMax = this.bMarks.length - 1; // don't count last fake line
}
```
- example usage
```shell
...
 * Process input string and push block tokens into 'outTokens'
 **/
ParserBlock.prototype.parse = function (src, md, env, outTokens) {
  var state;

  if (!src) { return; }

  state = new this.State(src, md, env, outTokens);

  this.tokenize(state, state.line, state.lineMax);
};


ParserBlock.prototype.State = require('./rules_block/state_block');
...
```

#### <a name="apidoc.element.markdown-it.parser_block.prototype.parse"></a>[function <span class="apidocSignatureSpan">markdown-it.parser_block.prototype.</span>parse (src, md, env, outTokens)](#apidoc.element.markdown-it.parser_block.prototype.parse)
- description and source-code
```javascript
parse = function (src, md, env, outTokens) {
  var state;

  if (!src) { return; }

  state = new this.State(src, md, env, outTokens);

  this.tokenize(state, state.line, state.lineMax);
}
```
- example usage
```shell
...
    state.line = line;
  }
}
};


/**
 * ParserBlock.parse(str, md, env, outTokens)
 *
 * Process input string and push block tokens into 'outTokens'
 **/
ParserBlock.prototype.parse = function (src, md, env, outTokens) {
var state;

if (!src) { return; }
...
```

#### <a name="apidoc.element.markdown-it.parser_block.prototype.tokenize"></a>[function <span class="apidocSignatureSpan">markdown-it.parser_block.prototype.</span>tokenize (state, startLine, endLine)](#apidoc.element.markdown-it.parser_block.prototype.tokenize)
- description and source-code
```javascript
tokenize = function (state, startLine, endLine) {
  var ok, i,
      rules = this.ruler.getRules(''),
      len = rules.length,
      line = startLine,
      hasEmptyLines = false,
      maxNesting = state.md.options.maxNesting;

  while (line < endLine) {
    state.line = line = state.skipEmptyLines(line);
    if (line >= endLine) { break; }

    // Termination condition for nested calls.
    // Nested calls currently used for blockquotes & lists
    if (state.sCount[line] < state.blkIndent) { break; }

    // If nesting level exceeded - skip tail to the end. That's not ordinary
    // situation and we should not care about content.
    if (state.level >= maxNesting) {
      state.line = endLine;
      break;
    }

    // Try all possible rules.
    // On success, rule should:
    //
    // - update 'state.line'
    // - update 'state.tokens'
    // - return true

    for (i = 0; i < len; i++) {
      ok = rules[i](state, line, endLine, false);
      if (ok) { break; }
    }

    // set state.tight iff we had an empty line before current tag
    // i.e. latest empty line should not count
    state.tight = !hasEmptyLines;

    // paragraph might "eat" one newline after it in nested lists
    if (state.isEmpty(state.line - 1)) {
      hasEmptyLines = true;
    }

    line = state.line;

    if (line < endLine && state.isEmpty(line)) {
      hasEmptyLines = true;
      line++;
      state.line = line;
    }
  }
}
```
- example usage
```shell
...
ParserBlock.prototype.parse = function (src, md, env, outTokens) {
  var state;

  if (!src) { return; }

  state = new this.State(src, md, env, outTokens);

  this.tokenize(state, state.line, state.lineMax);
};


ParserBlock.prototype.State = require('./rules_block/state_block');


module.exports = ParserBlock;
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
