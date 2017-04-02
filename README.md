# api documentation for  [markdown-it (v8.3.1)](https://github.com/markdown-it/markdown-it#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-markdown-it.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-markdown-it) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-markdown-it.svg)](https://travis-ci.org/npmdoc/node-npmdoc-markdown-it)
#### Markdown-it - modern pluggable markdown parser.

[![NPM](https://nodei.co/npm/markdown-it.png?downloads=true)](https://www.npmjs.com/package/markdown-it)

[![apidoc](https://npmdoc.github.io/node-npmdoc-markdown-it/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-markdown-it_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-markdown-it/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-markdown-it/build/screen-capture.npmPackageListing.svg)



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
            "name": "vitaly",
            "email": "vitaly@rcdesign.ru"
        }
    ],
    "name": "markdown-it",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
1.  [function <span class="apidocSignatureSpan">markdown-it.</span>parser_block ()](#apidoc.element.markdown-it.parser_block)
1.  [function <span class="apidocSignatureSpan">markdown-it.</span>parser_core ()](#apidoc.element.markdown-it.parser_core)
1.  [function <span class="apidocSignatureSpan">markdown-it.</span>parser_inline ()](#apidoc.element.markdown-it.parser_inline)
1.  [function <span class="apidocSignatureSpan">markdown-it.</span>renderer ()](#apidoc.element.markdown-it.renderer)
1.  [function <span class="apidocSignatureSpan">markdown-it.</span>ruler ()](#apidoc.element.markdown-it.ruler)
1.  [function <span class="apidocSignatureSpan">markdown-it.</span>token (type, tag, nesting)](#apidoc.element.markdown-it.token)
1.  object <span class="apidocSignatureSpan">markdown-it.</span>parser_block.prototype
1.  object <span class="apidocSignatureSpan">markdown-it.</span>parser_core.prototype
1.  object <span class="apidocSignatureSpan">markdown-it.</span>parser_inline.prototype
1.  object <span class="apidocSignatureSpan">markdown-it.</span>renderer.prototype
1.  object <span class="apidocSignatureSpan">markdown-it.</span>ruler.prototype
1.  object <span class="apidocSignatureSpan">markdown-it.</span>token.prototype

#### [module markdown-it.parser_block](#apidoc.module.markdown-it.parser_block)
1.  [function <span class="apidocSignatureSpan">markdown-it.</span>parser_block ()](#apidoc.element.markdown-it.parser_block.parser_block)

#### [module markdown-it.parser_block.prototype](#apidoc.module.markdown-it.parser_block.prototype)
1.  [function <span class="apidocSignatureSpan">markdown-it.parser_block.prototype.</span>State (src, md, env, tokens)](#apidoc.element.markdown-it.parser_block.prototype.State)
1.  [function <span class="apidocSignatureSpan">markdown-it.parser_block.prototype.</span>parse (src, md, env, outTokens)](#apidoc.element.markdown-it.parser_block.prototype.parse)
1.  [function <span class="apidocSignatureSpan">markdown-it.parser_block.prototype.</span>tokenize (state, startLine, endLine)](#apidoc.element.markdown-it.parser_block.prototype.tokenize)

#### [module markdown-it.parser_core](#apidoc.module.markdown-it.parser_core)
1.  [function <span class="apidocSignatureSpan">markdown-it.</span>parser_core ()](#apidoc.element.markdown-it.parser_core.parser_core)

#### [module markdown-it.parser_core.prototype](#apidoc.module.markdown-it.parser_core.prototype)
1.  [function <span class="apidocSignatureSpan">markdown-it.parser_core.prototype.</span>State (src, md, env)](#apidoc.element.markdown-it.parser_core.prototype.State)
1.  [function <span class="apidocSignatureSpan">markdown-it.parser_core.prototype.</span>process (state)](#apidoc.element.markdown-it.parser_core.prototype.process)

#### [module markdown-it.parser_inline](#apidoc.module.markdown-it.parser_inline)
1.  [function <span class="apidocSignatureSpan">markdown-it.</span>parser_inline ()](#apidoc.element.markdown-it.parser_inline.parser_inline)

#### [module markdown-it.parser_inline.prototype](#apidoc.module.markdown-it.parser_inline.prototype)
1.  [function <span class="apidocSignatureSpan">markdown-it.parser_inline.prototype.</span>State (src, md, env, outTokens)](#apidoc.element.markdown-it.parser_inline.prototype.State)
1.  [function <span class="apidocSignatureSpan">markdown-it.parser_inline.prototype.</span>parse (str, md, env, outTokens)](#apidoc.element.markdown-it.parser_inline.prototype.parse)
1.  [function <span class="apidocSignatureSpan">markdown-it.parser_inline.prototype.</span>skipToken (state)](#apidoc.element.markdown-it.parser_inline.prototype.skipToken)
1.  [function <span class="apidocSignatureSpan">markdown-it.parser_inline.prototype.</span>tokenize (state)](#apidoc.element.markdown-it.parser_inline.prototype.tokenize)

#### [module markdown-it.renderer](#apidoc.module.markdown-it.renderer)
1.  [function <span class="apidocSignatureSpan">markdown-it.</span>renderer ()](#apidoc.element.markdown-it.renderer.renderer)

#### [module markdown-it.renderer.prototype](#apidoc.module.markdown-it.renderer.prototype)
1.  [function <span class="apidocSignatureSpan">markdown-it.renderer.prototype.</span>render (tokens, options, env)](#apidoc.element.markdown-it.renderer.prototype.render)
1.  [function <span class="apidocSignatureSpan">markdown-it.renderer.prototype.</span>renderAttrs (token)](#apidoc.element.markdown-it.renderer.prototype.renderAttrs)
1.  [function <span class="apidocSignatureSpan">markdown-it.renderer.prototype.</span>renderInline (tokens, options, env)](#apidoc.element.markdown-it.renderer.prototype.renderInline)
1.  [function <span class="apidocSignatureSpan">markdown-it.renderer.prototype.</span>renderInlineAsText (tokens, options, env)](#apidoc.element.markdown-it.renderer.prototype.renderInlineAsText)
1.  [function <span class="apidocSignatureSpan">markdown-it.renderer.prototype.</span>renderToken (tokens, idx, options)](#apidoc.element.markdown-it.renderer.prototype.renderToken)

#### [module markdown-it.ruler](#apidoc.module.markdown-it.ruler)
1.  [function <span class="apidocSignatureSpan">markdown-it.</span>ruler ()](#apidoc.element.markdown-it.ruler.ruler)

#### [module markdown-it.ruler.prototype](#apidoc.module.markdown-it.ruler.prototype)
1.  [function <span class="apidocSignatureSpan">markdown-it.ruler.prototype.</span>__compile__ ()](#apidoc.element.markdown-it.ruler.prototype.__compile__)
1.  [function <span class="apidocSignatureSpan">markdown-it.ruler.prototype.</span>__find__ (name)](#apidoc.element.markdown-it.ruler.prototype.__find__)
1.  [function <span class="apidocSignatureSpan">markdown-it.ruler.prototype.</span>after (afterName, ruleName, fn, options)](#apidoc.element.markdown-it.ruler.prototype.after)
1.  [function <span class="apidocSignatureSpan">markdown-it.ruler.prototype.</span>at (name, fn, options)](#apidoc.element.markdown-it.ruler.prototype.at)
1.  [function <span class="apidocSignatureSpan">markdown-it.ruler.prototype.</span>before (beforeName, ruleName, fn, options)](#apidoc.element.markdown-it.ruler.prototype.before)
1.  [function <span class="apidocSignatureSpan">markdown-it.ruler.prototype.</span>disable (list, ignoreInvalid)](#apidoc.element.markdown-it.ruler.prototype.disable)
1.  [function <span class="apidocSignatureSpan">markdown-it.ruler.prototype.</span>enable (list, ignoreInvalid)](#apidoc.element.markdown-it.ruler.prototype.enable)
1.  [function <span class="apidocSignatureSpan">markdown-it.ruler.prototype.</span>enableOnly (list, ignoreInvalid)](#apidoc.element.markdown-it.ruler.prototype.enableOnly)
1.  [function <span class="apidocSignatureSpan">markdown-it.ruler.prototype.</span>getRules (chainName)](#apidoc.element.markdown-it.ruler.prototype.getRules)
1.  [function <span class="apidocSignatureSpan">markdown-it.ruler.prototype.</span>push (ruleName, fn, options)](#apidoc.element.markdown-it.ruler.prototype.push)

#### [module markdown-it.token](#apidoc.module.markdown-it.token)
1.  [function <span class="apidocSignatureSpan">markdown-it.</span>token (type, tag, nesting)](#apidoc.element.markdown-it.token.token)

#### [module markdown-it.token.prototype](#apidoc.module.markdown-it.token.prototype)
1.  [function <span class="apidocSignatureSpan">markdown-it.token.prototype.</span>attrGet (name)](#apidoc.element.markdown-it.token.prototype.attrGet)
1.  [function <span class="apidocSignatureSpan">markdown-it.token.prototype.</span>attrIndex (name)](#apidoc.element.markdown-it.token.prototype.attrIndex)
1.  [function <span class="apidocSignatureSpan">markdown-it.token.prototype.</span>attrJoin (name, value)](#apidoc.element.markdown-it.token.prototype.attrJoin)
1.  [function <span class="apidocSignatureSpan">markdown-it.token.prototype.</span>attrPush (attrData)](#apidoc.element.markdown-it.token.prototype.attrPush)
1.  [function <span class="apidocSignatureSpan">markdown-it.token.prototype.</span>attrSet (name, value)](#apidoc.element.markdown-it.token.prototype.attrSet)



# <a name="apidoc.module.markdown-it"></a>[module markdown-it](#apidoc.module.markdown-it)

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

#### <a name="apidoc.element.markdown-it.parser_core"></a>[function <span class="apidocSignatureSpan">markdown-it.</span>parser_core ()](#apidoc.element.markdown-it.parser_core)
- description and source-code
```javascript
function Core() {
<span class="apidocCodeCommentSpan">  /**
   * Core#ruler -> Ruler
   *
   * [[Ruler]] instance. Keep configuration of core rules.
   **/
</span>  this.ruler = new Ruler();

  for (var i = 0; i < _rules.length; i++) {
    this.ruler.push(_rules[i][0], _rules[i][1]);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.markdown-it.parser_inline"></a>[function <span class="apidocSignatureSpan">markdown-it.</span>parser_inline ()](#apidoc.element.markdown-it.parser_inline)
- description and source-code
```javascript
function ParserInline() {
  var i;

<span class="apidocCodeCommentSpan">  /**
   * ParserInline#ruler -> Ruler
   *
   * [[Ruler]] instance. Keep configuration of inline rules.
   **/
</span>  this.ruler = new Ruler();

  for (i = 0; i < _rules.length; i++) {
    this.ruler.push(_rules[i][0], _rules[i][1]);
  }

  /**
   * ParserInline#ruler2 -> Ruler
   *
   * [[Ruler]] instance. Second ruler used for post-processing
   * (e.g. in emphasis-like rules).
   **/
  this.ruler2 = new Ruler();

  for (i = 0; i < _rules2.length; i++) {
    this.ruler2.push(_rules2[i][0], _rules2[i][1]);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.markdown-it.renderer"></a>[function <span class="apidocSignatureSpan">markdown-it.</span>renderer ()](#apidoc.element.markdown-it.renderer)
- description and source-code
```javascript
function Renderer() {

<span class="apidocCodeCommentSpan">  /**
   * Renderer#rules -> Object
   *
   * Contains render rules for tokens. Can be updated and extended.
   *
   * ##### Example
   *
   * '''javascript
   * var md = require('markdown-it')();
   *
   * md.renderer.rules.strong_open  = function () { return '<b>'; };
   * md.renderer.rules.strong_close = function () { return '</b>'; };
   *
   * var result = md.renderInline(...);
   * '''
   *
   * Each rule is called as independed static function with fixed signature:
   *
   * '''javascript
   * function my_token_render(tokens, idx, options, env, renderer) {
   *   // ...
   *   return renderedHTML;
   * }
   * '''
   *
   * See [source code](https://github.com/markdown-it/markdown-it/blob/master/lib/renderer.js)
   * for more details and examples.
   **/
</span>  this.rules = assign({}, default_rules);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.markdown-it.ruler"></a>[function <span class="apidocSignatureSpan">markdown-it.</span>ruler ()](#apidoc.element.markdown-it.ruler)
- description and source-code
```javascript
function Ruler() {
  // List of added rules. Each element is:
  //
  // {
  //   name: XXX,
  //   enabled: Boolean,
  //   fn: Function(),
  //   alt: [ name2, name3 ]
  // }
  //
  this.__rules__ = [];

  // Cached rule chains.
  //
  // First level - chain name, '' for default.
  // Second level - diginal anchor for fast filtering by charcodes.
  //
  this.__cache__ = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.markdown-it.token"></a>[function <span class="apidocSignatureSpan">markdown-it.</span>token (type, tag, nesting)](#apidoc.element.markdown-it.token)
- description and source-code
```javascript
function Token(type, tag, nesting) {
<span class="apidocCodeCommentSpan">  /**
   * Token#type -> String
   *
   * Type of the token (string, e.g. "paragraph_open")
   **/
</span>  this.type     = type;

  /**
   * Token#tag -> String
   *
   * html tag name, e.g. "p"
   **/
  this.tag      = tag;

  /**
   * Token#attrs -> Array
   *
   * Html attributes. Format: '[ [ name1, value1 ], [ name2, value2 ] ]'
   **/
  this.attrs    = null;

  /**
   * Token#map -> Array
   *
   * Source map info. Format: '[ line_begin, line_end ]'
   **/
  this.map      = null;

  /**
   * Token#nesting -> Number
   *
   * Level change (number in {-1, 0, 1} set), where:
   *
   * -  '1' means the tag is opening
   * -  '0' means the tag is self-closing
   * - '-1' means the tag is closing
   **/
  this.nesting  = nesting;

  /**
   * Token#level -> Number
   *
   * nesting level, the same as 'state.level'
   **/
  this.level    = 0;

  /**
   * Token#children -> Array
   *
   * An array of child nodes (inline and img tokens)
   **/
  this.children = null;

  /**
   * Token#content -> String
   *
   * In a case of self-closing tag (code, html, fence, etc.),
   * it has contents of this tag.
   **/
  this.content  = '';

  /**
   * Token#markup -> String
   *
   * '*' or '_' for emphasis, fence string for fence, etc.
   **/
  this.markup   = '';

  /**
   * Token#info -> String
   *
   * fence infostring
   **/
  this.info     = '';

  /**
   * Token#meta -> Object
   *
   * A place for plugins to store an arbitrary data
   **/
  this.meta     = null;

  /**
   * Token#block -> Boolean
   *
   * True for block-level tokens, false for inline tokens.
   * Used in renderer to calculate line breaks
   **/
  this.block    = false;

  /**
   * Token#hidden -> Boolean
   *
   * If it's true, ignore this element when rendering. Used for tight lists
   * to hide paragraphs.
   **/
  this.hidden   = false;
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



# <a name="apidoc.module.markdown-it.parser_core"></a>[module markdown-it.parser_core](#apidoc.module.markdown-it.parser_core)

#### <a name="apidoc.element.markdown-it.parser_core.parser_core"></a>[function <span class="apidocSignatureSpan">markdown-it.</span>parser_core ()](#apidoc.element.markdown-it.parser_core.parser_core)
- description and source-code
```javascript
function Core() {
<span class="apidocCodeCommentSpan">  /**
   * Core#ruler -> Ruler
   *
   * [[Ruler]] instance. Keep configuration of core rules.
   **/
</span>  this.ruler = new Ruler();

  for (var i = 0; i < _rules.length; i++) {
    this.ruler.push(_rules[i][0], _rules[i][1]);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.markdown-it.parser_core.prototype"></a>[module markdown-it.parser_core.prototype](#apidoc.module.markdown-it.parser_core.prototype)

#### <a name="apidoc.element.markdown-it.parser_core.prototype.State"></a>[function <span class="apidocSignatureSpan">markdown-it.parser_core.prototype.</span>State (src, md, env)](#apidoc.element.markdown-it.parser_core.prototype.State)
- description and source-code
```javascript
function StateCore(src, md, env) {
  this.src = src;
  this.env = env;
  this.tokens = [];
  this.inlineMode = false;
  this.md = md; // link to parser instance
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

#### <a name="apidoc.element.markdown-it.parser_core.prototype.process"></a>[function <span class="apidocSignatureSpan">markdown-it.parser_core.prototype.</span>process (state)](#apidoc.element.markdown-it.parser_core.prototype.process)
- description and source-code
```javascript
process = function (state) {
  var i, l, rules;

  rules = this.ruler.getRules('');

  for (i = 0, l = rules.length; i < l; i++) {
    rules[i](state);
  }
}
```
- example usage
```shell
...
for (var i = 0; i < _rules.length; i++) {
  this.ruler.push(_rules[i][0], _rules[i][1]);
}
}


/**
 * Core.process(state)
 *
 * Executes core chain rules.
 **/
Core.prototype.process = function (state) {
var i, l, rules;

rules = this.ruler.getRules('');
...
```



# <a name="apidoc.module.markdown-it.parser_inline"></a>[module markdown-it.parser_inline](#apidoc.module.markdown-it.parser_inline)

#### <a name="apidoc.element.markdown-it.parser_inline.parser_inline"></a>[function <span class="apidocSignatureSpan">markdown-it.</span>parser_inline ()](#apidoc.element.markdown-it.parser_inline.parser_inline)
- description and source-code
```javascript
function ParserInline() {
  var i;

<span class="apidocCodeCommentSpan">  /**
   * ParserInline#ruler -> Ruler
   *
   * [[Ruler]] instance. Keep configuration of inline rules.
   **/
</span>  this.ruler = new Ruler();

  for (i = 0; i < _rules.length; i++) {
    this.ruler.push(_rules[i][0], _rules[i][1]);
  }

  /**
   * ParserInline#ruler2 -> Ruler
   *
   * [[Ruler]] instance. Second ruler used for post-processing
   * (e.g. in emphasis-like rules).
   **/
  this.ruler2 = new Ruler();

  for (i = 0; i < _rules2.length; i++) {
    this.ruler2.push(_rules2[i][0], _rules2[i][1]);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.markdown-it.parser_inline.prototype"></a>[module markdown-it.parser_inline.prototype](#apidoc.module.markdown-it.parser_inline.prototype)

#### <a name="apidoc.element.markdown-it.parser_inline.prototype.State"></a>[function <span class="apidocSignatureSpan">markdown-it.parser_inline.prototype.</span>State (src, md, env, outTokens)](#apidoc.element.markdown-it.parser_inline.prototype.State)
- description and source-code
```javascript
function StateInline(src, md, env, outTokens) {
  this.src = src;
  this.env = env;
  this.md = md;
  this.tokens = outTokens;

  this.pos = 0;
  this.posMax = this.src.length;
  this.level = 0;
  this.pending = '';
  this.pendingLevel = 0;

  this.cache = {};        // Stores { start: end } pairs. Useful for backtrack
                          // optimization of pairs parse (emphasis, strikes).

  this.delimiters = [];   // Emphasis-like delimiters
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

#### <a name="apidoc.element.markdown-it.parser_inline.prototype.parse"></a>[function <span class="apidocSignatureSpan">markdown-it.parser_inline.prototype.</span>parse (str, md, env, outTokens)](#apidoc.element.markdown-it.parser_inline.prototype.parse)
- description and source-code
```javascript
parse = function (str, md, env, outTokens) {
  var i, rules, len;
  var state = new this.State(str, md, env, outTokens);

  this.tokenize(state);

  rules = this.ruler2.getRules('');
  len = rules.length;

  for (i = 0; i < len; i++) {
    rules[i](state);
  }
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

#### <a name="apidoc.element.markdown-it.parser_inline.prototype.skipToken"></a>[function <span class="apidocSignatureSpan">markdown-it.parser_inline.prototype.</span>skipToken (state)](#apidoc.element.markdown-it.parser_inline.prototype.skipToken)
- description and source-code
```javascript
skipToken = function (state) {
  var ok, i, pos = state.pos,
      rules = this.ruler.getRules(''),
      len = rules.length,
      maxNesting = state.md.options.maxNesting,
      cache = state.cache;


  if (typeof cache[pos] !== 'undefined') {
    state.pos = cache[pos];
    return;
  }

  if (state.level < maxNesting) {
    for (i = 0; i < len; i++) {
      // Increment state.level and decrement it later to limit recursion.
      // It's harmless to do here, because no tokens are created. But ideally,
      // we'd need a separate private state variable for this purpose.
      //
      state.level++;
      ok = rules[i](state, true);
      state.level--;

      if (ok) { break; }
    }
  } else {
    // Too much nesting, just skip until the end of the paragraph.
    //
    // NOTE: this will cause links to behave incorrectly in the following case,
    //       when an amount of '[' is exactly equal to 'maxNesting + 1':
    //
    //       [[[[[[[[[[[[[[[[[[[[[foo]()
    //
    // TODO: remove this workaround when CM standard will allow nested links
    //       (we can replace it by preventing links from being parsed in
    //       validation mode)
    //
    state.pos = state.posMax;
  }

  if (!ok) { state.pos++; }
  cache[pos] = state.pos;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.markdown-it.parser_inline.prototype.tokenize"></a>[function <span class="apidocSignatureSpan">markdown-it.parser_inline.prototype.</span>tokenize (state)](#apidoc.element.markdown-it.parser_inline.prototype.tokenize)
- description and source-code
```javascript
tokenize = function (state) {
  var ok, i,
      rules = this.ruler.getRules(''),
      len = rules.length,
      end = state.posMax,
      maxNesting = state.md.options.maxNesting;

  while (state.pos < end) {
    // Try all possible rules.
    // On success, rule should:
    //
    // - update 'state.pos'
    // - update 'state.tokens'
    // - return true

    if (state.level < maxNesting) {
      for (i = 0; i < len; i++) {
        ok = rules[i](state, false);
        if (ok) { break; }
      }
    }

    if (ok) {
      if (state.pos >= end) { break; }
      continue;
    }

    state.pending += state.src[state.pos++];
  }

  if (state.pending) {
    state.pushPending();
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



# <a name="apidoc.module.markdown-it.renderer"></a>[module markdown-it.renderer](#apidoc.module.markdown-it.renderer)

#### <a name="apidoc.element.markdown-it.renderer.renderer"></a>[function <span class="apidocSignatureSpan">markdown-it.</span>renderer ()](#apidoc.element.markdown-it.renderer.renderer)
- description and source-code
```javascript
function Renderer() {

<span class="apidocCodeCommentSpan">  /**
   * Renderer#rules -> Object
   *
   * Contains render rules for tokens. Can be updated and extended.
   *
   * ##### Example
   *
   * '''javascript
   * var md = require('markdown-it')();
   *
   * md.renderer.rules.strong_open  = function () { return '<b>'; };
   * md.renderer.rules.strong_close = function () { return '</b>'; };
   *
   * var result = md.renderInline(...);
   * '''
   *
   * Each rule is called as independed static function with fixed signature:
   *
   * '''javascript
   * function my_token_render(tokens, idx, options, env, renderer) {
   *   // ...
   *   return renderedHTML;
   * }
   * '''
   *
   * See [source code](https://github.com/markdown-it/markdown-it/blob/master/lib/renderer.js)
   * for more details and examples.
   **/
</span>  this.rules = assign({}, default_rules);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.markdown-it.renderer.prototype"></a>[module markdown-it.renderer.prototype](#apidoc.module.markdown-it.renderer.prototype)

#### <a name="apidoc.element.markdown-it.renderer.prototype.render"></a>[function <span class="apidocSignatureSpan">markdown-it.renderer.prototype.</span>render (tokens, options, env)](#apidoc.element.markdown-it.renderer.prototype.render)
- description and source-code
```javascript
render = function (tokens, options, env) {
  var i, len, type,
      result = '',
      rules = this.rules;

  for (i = 0, len = tokens.length; i < len; i++) {
    type = tokens[i].type;

    if (type === 'inline') {
      result += this.renderInline(tokens[i].children, options, env);
    } else if (typeof rules[type] !== 'undefined') {
      result += rules[tokens[i].type](tokens, i, options, env, this);
    } else {
      result += this.renderToken(tokens, i, options, env);
    }
  }

  return result;
}
```
- example usage
```shell
...

### Simple

'''js
// node.js, "classic" way:
var MarkdownIt = require('markdown-it'),
    md = new MarkdownIt();
var result = md.render('# markdown-it rulezz!');

// node.js, the same, but with sugar:
var md = require('markdown-it')();
var result = md.render('# markdown-it rulezz!');

// browser without AMD, added to "window" on script load
// Note, there is no dash in "markdownit".
...
```

#### <a name="apidoc.element.markdown-it.renderer.prototype.renderAttrs"></a>[function <span class="apidocSignatureSpan">markdown-it.renderer.prototype.</span>renderAttrs (token)](#apidoc.element.markdown-it.renderer.prototype.renderAttrs)
- description and source-code
```javascript
function renderAttrs(token) {
  var i, l, result;

  if (!token.attrs) { return ''; }

  result = '';

  for (i = 0, l = token.attrs.length; i < l; i++) {
    result += ' ' + escapeHtml(token.attrs[i][0]) + '="' + escapeHtml(token.attrs[i][1]) + '"';
  }

  return result;
}
```
- example usage
```shell
...

var default_rules = {};


default_rules.code_inline = function (tokens, idx, options, env, slf) {
var token = tokens[idx];

return  '<code' + slf.renderAttrs(token) + '>' +
        escapeHtml(tokens[idx].content) +
        '</code>';
};


default_rules.code_block = function (tokens, idx, options, env, slf) {
var token = tokens[idx];
...
```

#### <a name="apidoc.element.markdown-it.renderer.prototype.renderInline"></a>[function <span class="apidocSignatureSpan">markdown-it.renderer.prototype.</span>renderInline (tokens, options, env)](#apidoc.element.markdown-it.renderer.prototype.renderInline)
- description and source-code
```javascript
renderInline = function (tokens, options, env) {
  var type,
      result = '',
      rules = this.rules;

  for (var i = 0, len = tokens.length; i < len; i++) {
    type = tokens[i].type;

    if (typeof rules[type] !== 'undefined') {
      result += rules[type](tokens, i, options, env, this);
    } else {
      result += this.renderToken(tokens, i, options);
    }
  }

  return result;
}
```
- example usage
```shell
...
var result = md.render('# markdown-it rulezz!');
'''

Single line rendering, without paragraph wrap:

'''js
var md = require('markdown-it')();
var result = md.renderInline('__markdown-it__ rulezz!');
'''


### Init with presets and options

(*) presets define combinations of active rules and options. Can be
'"commonmark"', '"zero"' or '"default"' (if skipped). See
...
```

#### <a name="apidoc.element.markdown-it.renderer.prototype.renderInlineAsText"></a>[function <span class="apidocSignatureSpan">markdown-it.renderer.prototype.</span>renderInlineAsText (tokens, options, env)](#apidoc.element.markdown-it.renderer.prototype.renderInlineAsText)
- description and source-code
```javascript
renderInlineAsText = function (tokens, options, env) {
  var result = '';

  for (var i = 0, len = tokens.length; i < len; i++) {
    if (tokens[i].type === 'text') {
      result += tokens[i].content;
    } else if (tokens[i].type === 'image') {
      result += this.renderInlineAsText(tokens[i].children, options, env);
    }
  }

  return result;
}
```
- example usage
```shell
...

// "alt" attr MUST be set, even if empty. Because it's mandatory and
// should be placed on proper position for tests.
//
// Replace content with actual value

token.attrs[token.attrIndex('alt')][1] =
  slf.renderInlineAsText(token.children, options, env);

return slf.renderToken(tokens, idx, options);
};


default_rules.hardbreak = function (tokens, idx, options /*, env */) {
return options.xhtmlOut ? '<br />\n' : '<br>\n';
...
```

#### <a name="apidoc.element.markdown-it.renderer.prototype.renderToken"></a>[function <span class="apidocSignatureSpan">markdown-it.renderer.prototype.</span>renderToken (tokens, idx, options)](#apidoc.element.markdown-it.renderer.prototype.renderToken)
- description and source-code
```javascript
function renderToken(tokens, idx, options) {
  var nextToken,
      result = '',
      needLf = false,
      token = tokens[idx];

  // Tight list paragraphs
  if (token.hidden) {
    return '';
  }

  // Insert a newline between hidden paragraph and subsequent opening
  // block-level tag.
  //
  // For example, here we should insert a newline before blockquote:
  //  - a
  //    >
  //
  if (token.block && token.nesting !== -1 && idx && tokens[idx - 1].hidden) {
    result += '\n';
  }

  // Add token name, e.g. '<img'
  result += (token.nesting === -1 ? '</' : '<') + token.tag;

  // Encode attributes, e.g. '<img src="foo"'
  result += this.renderAttrs(token);

  // Add a slash for self-closing tags, e.g. '<img src="foo" /'
  if (token.nesting === 0 && options.xhtmlOut) {
    result += ' /';
  }

  // Check if we need to add a newline after this tag
  if (token.block) {
    needLf = true;

    if (token.nesting === 1) {
      if (idx + 1 < tokens.length) {
        nextToken = tokens[idx + 1];

        if (nextToken.type === 'inline' || nextToken.hidden) {
          // Block-level tag containing an inline tag.
          //
          needLf = false;

        } else if (nextToken.nesting === -1 && nextToken.tag === token.tag) {
          // Opening tag + closing tag of the same type. E.g. '<li></li>'.
          //
          needLf = false;
        }
      }
    }
  }

  result += needLf ? '>\n' : '>';

  return result;
}
```
- example usage
```shell
...
  // should be placed on proper position for tests.
  //
  // Replace content with actual value

  token.attrs[token.attrIndex('alt')][1] =
    slf.renderInlineAsText(token.children, options, env);

  return slf.renderToken(tokens, idx, options);
};


default_rules.hardbreak = function (tokens, idx, options /*, env */) {
  return options.xhtmlOut ? '<br />\n' : '<br>\n';
};
default_rules.softbreak = function (tokens, idx, options /*, env */) {
...
```



# <a name="apidoc.module.markdown-it.ruler"></a>[module markdown-it.ruler](#apidoc.module.markdown-it.ruler)

#### <a name="apidoc.element.markdown-it.ruler.ruler"></a>[function <span class="apidocSignatureSpan">markdown-it.</span>ruler ()](#apidoc.element.markdown-it.ruler.ruler)
- description and source-code
```javascript
function Ruler() {
  // List of added rules. Each element is:
  //
  // {
  //   name: XXX,
  //   enabled: Boolean,
  //   fn: Function(),
  //   alt: [ name2, name3 ]
  // }
  //
  this.__rules__ = [];

  // Cached rule chains.
  //
  // First level - chain name, '' for default.
  // Second level - diginal anchor for fast filtering by charcodes.
  //
  this.__cache__ = null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.markdown-it.ruler.prototype"></a>[module markdown-it.ruler.prototype](#apidoc.module.markdown-it.ruler.prototype)

#### <a name="apidoc.element.markdown-it.ruler.prototype.__compile__"></a>[function <span class="apidocSignatureSpan">markdown-it.ruler.prototype.</span>__compile__ ()](#apidoc.element.markdown-it.ruler.prototype.__compile__)
- description and source-code
```javascript
__compile__ = function () {
  var self = this;
  var chains = [ '' ];

  // collect unique names
  self.__rules__.forEach(function (rule) {
    if (!rule.enabled) { return; }

    rule.alt.forEach(function (altName) {
      if (chains.indexOf(altName) < 0) {
        chains.push(altName);
      }
    });
  });

  self.__cache__ = {};

  chains.forEach(function (chain) {
    self.__cache__[chain] = [];
    self.__rules__.forEach(function (rule) {
      if (!rule.enabled) { return; }

      if (chain && rule.alt.indexOf(chain) < 0) { return; }

      self.__cache__[chain].push(rule.fn);
    });
  });
}
```
- example usage
```shell
...
 * rules configuration, compiles caches if not exists and returns result.
 *
 * Default chain name is '''' (empty string). It can't be skipped. That's
 * done intentionally, to keep signature monomorphic for high speed.
 **/
Ruler.prototype.getRules = function (chainName) {
  if (this.__cache__ === null) {
    this.__compile__();
  }

  // Chain can be empty, if rules disabled. But we still have to return Array.
  return this.__cache__[chainName] || [];
};

module.exports = Ruler;
...
```

#### <a name="apidoc.element.markdown-it.ruler.prototype.__find__"></a>[function <span class="apidocSignatureSpan">markdown-it.ruler.prototype.</span>__find__ (name)](#apidoc.element.markdown-it.ruler.prototype.__find__)
- description and source-code
```javascript
__find__ = function (name) {
  for (var i = 0; i < this.__rules__.length; i++) {
    if (this.__rules__[i].name === name) {
      return i;
    }
  }
  return -1;
}
```
- example usage
```shell
...
 *
 * md.core.ruler.at('replacements', function replace(state) {
 *   //...
 * });
 * '''
 **/
Ruler.prototype.at = function (name, fn, options) {
var index = this.__find__(name);
var opt = options || {};

if (index === -1) { throw new Error('Parser rule not found: ' + name); }

this.__rules__[index].fn = fn;
this.__rules__[index].alt = opt.alt || [];
this.__cache__ = null;
...
```

#### <a name="apidoc.element.markdown-it.ruler.prototype.after"></a>[function <span class="apidocSignatureSpan">markdown-it.ruler.prototype.</span>after (afterName, ruleName, fn, options)](#apidoc.element.markdown-it.ruler.prototype.after)
- description and source-code
```javascript
after = function (afterName, ruleName, fn, options) {
  var index = this.__find__(afterName);
  var opt = options || {};

  if (index === -1) { throw new Error('Parser rule not found: ' + afterName); }

  this.__rules__.splice(index + 1, 0, {
    name: ruleName,
    enabled: true,
    fn: fn,
    alt: opt.alt || []
  });

  this.__cache__ = null;
}
```
- example usage
```shell
...
 });

 this.__cache__ = null;
};


/**
* Ruler.after(afterName, ruleName, fn [, options])
* - afterName (String): new rule will be added after this one.
* - ruleName (String): name of added rule.
* - fn (Function): rule function.
* - options (Object): rule options (not mandatory).
*
* Add new rule to chain after one with given name. See also
* [[Ruler.before]], [[Ruler.push]].
...
```

#### <a name="apidoc.element.markdown-it.ruler.prototype.at"></a>[function <span class="apidocSignatureSpan">markdown-it.ruler.prototype.</span>at (name, fn, options)](#apidoc.element.markdown-it.ruler.prototype.at)
- description and source-code
```javascript
at = function (name, fn, options) {
  var index = this.__find__(name);
  var opt = options || {};

  if (index === -1) { throw new Error('Parser rule not found: ' + name); }

  this.__rules__[index].fn = fn;
  this.__rules__[index].alt = opt.alt || [];
  this.__cache__ = null;
}
```
- example usage
```shell
...
     self.__cache__[chain].push(rule.fn);
   });
 });
};


/**
* Ruler.at(name, fn [, options])
* - name (String): rule name to replace.
* - fn (Function): new rule function.
* - options (Object): new rule options (not mandatory).
*
* Replace rule by name with new function & options. Throws error if name not
* found.
*
...
```

#### <a name="apidoc.element.markdown-it.ruler.prototype.before"></a>[function <span class="apidocSignatureSpan">markdown-it.ruler.prototype.</span>before (beforeName, ruleName, fn, options)](#apidoc.element.markdown-it.ruler.prototype.before)
- description and source-code
```javascript
before = function (beforeName, ruleName, fn, options) {
  var index = this.__find__(beforeName);
  var opt = options || {};

  if (index === -1) { throw new Error('Parser rule not found: ' + beforeName); }

  this.__rules__.splice(index, 0, {
    name: ruleName,
    enabled: true,
    fn: fn,
    alt: opt.alt || []
  });

  this.__cache__ = null;
}
```
- example usage
```shell
...
 this.__rules__[index].fn = fn;
 this.__rules__[index].alt = opt.alt || [];
 this.__cache__ = null;
};


/**
* Ruler.before(beforeName, ruleName, fn [, options])
* - beforeName (String): new rule will be added before this one.
* - ruleName (String): name of added rule.
* - fn (Function): rule function.
* - options (Object): rule options (not mandatory).
*
* Add new rule to chain before one with given name. See also
* [[Ruler.after]], [[Ruler.push]].
...
```

#### <a name="apidoc.element.markdown-it.ruler.prototype.disable"></a>[function <span class="apidocSignatureSpan">markdown-it.ruler.prototype.</span>disable (list, ignoreInvalid)](#apidoc.element.markdown-it.ruler.prototype.disable)
- description and source-code
```javascript
disable = function (list, ignoreInvalid) {
  if (!Array.isArray(list)) { list = [ list ]; }

  var result = [];

  // Search by name and disable
  list.forEach(function (name) {
    var idx = this.__find__(name);

    if (idx < 0) {
      if (ignoreInvalid) { return; }
      throw new Error('Rules manager: invalid rule name ' + name);
    }
    this.__rules__[idx].enabled = false;
    result.push(name);
  }, this);

  this.__cache__ = null;
  return result;
}
```
- example usage
```shell
...

By default all rules are enabled, but can be restricted by options. On plugin
load all its rules are enabled automatically.

'''js
// Activate/deactivate rules, with curring
var md = require('markdown-it')()
          .disable([ 'link', 'image' ])
          .enable([ 'link' ])
          .enable('image');

// Enable everything
md = require('markdown-it')({
html: true,
linkify: true,
...
```

#### <a name="apidoc.element.markdown-it.ruler.prototype.enable"></a>[function <span class="apidocSignatureSpan">markdown-it.ruler.prototype.</span>enable (list, ignoreInvalid)](#apidoc.element.markdown-it.ruler.prototype.enable)
- description and source-code
```javascript
enable = function (list, ignoreInvalid) {
  if (!Array.isArray(list)) { list = [ list ]; }

  var result = [];

  // Search by name and enable
  list.forEach(function (name) {
    var idx = this.__find__(name);

    if (idx < 0) {
      if (ignoreInvalid) { return; }
      throw new Error('Rules manager: invalid rule name ' + name);
    }
    this.__rules__[idx].enabled = true;
    result.push(name);
  }, this);

  this.__cache__ = null;
  return result;
}
```
- example usage
```shell
...
By default all rules are enabled, but can be restricted by options. On plugin
load all its rules are enabled automatically.

'''js
// Activate/deactivate rules, with curring
var md = require('markdown-it')()
          .disable([ 'link', 'image' ])
          .enable([ 'link' ])
          .enable('image');

// Enable everything
md = require('markdown-it')({
html: true,
linkify: true,
typographer: true,
...
```

#### <a name="apidoc.element.markdown-it.ruler.prototype.enableOnly"></a>[function <span class="apidocSignatureSpan">markdown-it.ruler.prototype.</span>enableOnly (list, ignoreInvalid)](#apidoc.element.markdown-it.ruler.prototype.enableOnly)
- description and source-code
```javascript
enableOnly = function (list, ignoreInvalid) {
  if (!Array.isArray(list)) { list = [ list ]; }

  this.__rules__.forEach(function (rule) { rule.enabled = false; });

  this.enable(list, ignoreInvalid);
}
```
- example usage
```shell
...

 this.__cache__ = null;
 return result;
};


/**
* Ruler.enableOnly(list [, ignoreInvalid])
* - list (String|Array): list of rule names to enable (whitelist).
* - ignoreInvalid (Boolean): set 'true' to ignore errors when rule not found.
*
* Enable rules with given names, and disable everything else. If any rule name
* not found - throw Error. Errors can be disabled by second param.
*
* See also [[Ruler.disable]], [[Ruler.enable]].
...
```

#### <a name="apidoc.element.markdown-it.ruler.prototype.getRules"></a>[function <span class="apidocSignatureSpan">markdown-it.ruler.prototype.</span>getRules (chainName)](#apidoc.element.markdown-it.ruler.prototype.getRules)
- description and source-code
```javascript
getRules = function (chainName) {
  if (this.__cache__ === null) {
    this.__compile__();
  }

  // Chain can be empty, if rules disabled. But we still have to return Array.
  return this.__cache__[chainName] || [];
}
```
- example usage
```shell
...
}


// Generate tokens for input range
//
ParserBlock.prototype.tokenize = function (state, startLine, endLine) {
var ok, i,
    rules = this.ruler.getRules(''),
    len = rules.length,
    line = startLine,
    hasEmptyLines = false,
    maxNesting = state.md.options.maxNesting;

while (line < endLine) {
  state.line = line = state.skipEmptyLines(line);
...
```

#### <a name="apidoc.element.markdown-it.ruler.prototype.push"></a>[function <span class="apidocSignatureSpan">markdown-it.ruler.prototype.</span>push (ruleName, fn, options)](#apidoc.element.markdown-it.ruler.prototype.push)
- description and source-code
```javascript
push = function (ruleName, fn, options) {
  var opt = options || {};

  this.__rules__.push({
    name: ruleName,
    enabled: true,
    fn: fn,
    alt: opt.alt || []
  });

  this.__cache__ = null;
}
```
- example usage
```shell
...
   * ParserBlock#ruler -> Ruler
   *
   * [[Ruler]] instance. Keep configuration of block rules.
   **/
  this.ruler = new Ruler();

  for (var i = 0; i < _rules.length; i++) {
    this.ruler.push(_rules[i][0], _rules[i][1], { alt: (_rules[i][2] || []).slice() });
  }
}


// Generate tokens for input range
//
ParserBlock.prototype.tokenize = function (state, startLine, endLine) {
...
```



# <a name="apidoc.module.markdown-it.token"></a>[module markdown-it.token](#apidoc.module.markdown-it.token)

#### <a name="apidoc.element.markdown-it.token.token"></a>[function <span class="apidocSignatureSpan">markdown-it.</span>token (type, tag, nesting)](#apidoc.element.markdown-it.token.token)
- description and source-code
```javascript
function Token(type, tag, nesting) {
<span class="apidocCodeCommentSpan">  /**
   * Token#type -> String
   *
   * Type of the token (string, e.g. "paragraph_open")
   **/
</span>  this.type     = type;

  /**
   * Token#tag -> String
   *
   * html tag name, e.g. "p"
   **/
  this.tag      = tag;

  /**
   * Token#attrs -> Array
   *
   * Html attributes. Format: '[ [ name1, value1 ], [ name2, value2 ] ]'
   **/
  this.attrs    = null;

  /**
   * Token#map -> Array
   *
   * Source map info. Format: '[ line_begin, line_end ]'
   **/
  this.map      = null;

  /**
   * Token#nesting -> Number
   *
   * Level change (number in {-1, 0, 1} set), where:
   *
   * -  '1' means the tag is opening
   * -  '0' means the tag is self-closing
   * - '-1' means the tag is closing
   **/
  this.nesting  = nesting;

  /**
   * Token#level -> Number
   *
   * nesting level, the same as 'state.level'
   **/
  this.level    = 0;

  /**
   * Token#children -> Array
   *
   * An array of child nodes (inline and img tokens)
   **/
  this.children = null;

  /**
   * Token#content -> String
   *
   * In a case of self-closing tag (code, html, fence, etc.),
   * it has contents of this tag.
   **/
  this.content  = '';

  /**
   * Token#markup -> String
   *
   * '*' or '_' for emphasis, fence string for fence, etc.
   **/
  this.markup   = '';

  /**
   * Token#info -> String
   *
   * fence infostring
   **/
  this.info     = '';

  /**
   * Token#meta -> Object
   *
   * A place for plugins to store an arbitrary data
   **/
  this.meta     = null;

  /**
   * Token#block -> Boolean
   *
   * True for block-level tokens, false for inline tokens.
   * Used in renderer to calculate line breaks
   **/
  this.block    = false;

  /**
   * Token#hidden -> Boolean
   *
   * If it's true, ignore this element when rendering. Used for tight lists
   * to hide paragraphs.
   **/
  this.hidden   = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.markdown-it.token.prototype"></a>[module markdown-it.token.prototype](#apidoc.module.markdown-it.token.prototype)

#### <a name="apidoc.element.markdown-it.token.prototype.attrGet"></a>[function <span class="apidocSignatureSpan">markdown-it.token.prototype.</span>attrGet (name)](#apidoc.element.markdown-it.token.prototype.attrGet)
- description and source-code
```javascript
function attrGet(name) {
  var idx = this.attrIndex(name), value = null;
  if (idx >= 0) {
    value = this.attrs[idx][1];
  }
  return value;
}
```
- example usage
```shell
...
} else {
  this.attrs[idx] = attrData;
}
};


/**
 * Token.attrGet(name)
 *
 * Get the value of attribute 'name', or null if it does not exist.
 **/
Token.prototype.attrGet = function attrGet(name) {
var idx = this.attrIndex(name), value = null;
if (idx >= 0) {
  value = this.attrs[idx][1];
...
```

#### <a name="apidoc.element.markdown-it.token.prototype.attrIndex"></a>[function <span class="apidocSignatureSpan">markdown-it.token.prototype.</span>attrIndex (name)](#apidoc.element.markdown-it.token.prototype.attrIndex)
- description and source-code
```javascript
function attrIndex(name) {
  var attrs, i, len;

  if (!this.attrs) { return -1; }

  attrs = this.attrs;

  for (i = 0, len = attrs.length; i < len; i++) {
    if (attrs[i][0] === name) { return i; }
  }
  return -1;
}
```
- example usage
```shell
...
return highlighted + '\n';
  }

  // If language exists, inject class gently, without mudofying original token.
  // May be, one day we will add .clone() for token and simplify this part, but
  // now we prefer to keep things local.
  if (info) {
i        = token.attrIndex('class');
tmpAttrs = token.attrs ? token.attrs.slice() : [];

if (i < 0) {
  tmpAttrs.push([ 'class', options.langPrefix + langName ]);
} else {
  tmpAttrs[i][1] += ' ' + options.langPrefix + langName;
}
...
```

#### <a name="apidoc.element.markdown-it.token.prototype.attrJoin"></a>[function <span class="apidocSignatureSpan">markdown-it.token.prototype.</span>attrJoin (name, value)](#apidoc.element.markdown-it.token.prototype.attrJoin)
- description and source-code
```javascript
function attrJoin(name, value) {
  var idx = this.attrIndex(name);

  if (idx < 0) {
    this.attrPush([ name, value ]);
  } else {
    this.attrs[idx][1] = this.attrs[idx][1] + ' ' + value;
  }
}
```
- example usage
```shell
...
  value = this.attrs[idx][1];
}
return value;
};


/**
 * Token.attrJoin(name, value)
 *
 * Join value to existing attribute via space. Or create new attribute if not
 * exists. Useful to operate with token classes.
 **/
Token.prototype.attrJoin = function attrJoin(name, value) {
var idx = this.attrIndex(name);
...
```

#### <a name="apidoc.element.markdown-it.token.prototype.attrPush"></a>[function <span class="apidocSignatureSpan">markdown-it.token.prototype.</span>attrPush (attrData)](#apidoc.element.markdown-it.token.prototype.attrPush)
- description and source-code
```javascript
function attrPush(attrData) {
  if (this.attrs) {
    this.attrs.push(attrData);
  } else {
    this.attrs = [ attrData ];
  }
}
```
- example usage
```shell
...
  if (attrs[i][0] === name) { return i; }
}
return -1;
};


/**
 * Token.attrPush(attrData)
 *
 * Add '[ name, value ]' attribute to list. Init attrs if necessary
 **/
Token.prototype.attrPush = function attrPush(attrData) {
if (this.attrs) {
  this.attrs.push(attrData);
} else {
...
```

#### <a name="apidoc.element.markdown-it.token.prototype.attrSet"></a>[function <span class="apidocSignatureSpan">markdown-it.token.prototype.</span>attrSet (name, value)](#apidoc.element.markdown-it.token.prototype.attrSet)
- description and source-code
```javascript
function attrSet(name, value) {
  var idx = this.attrIndex(name),
      attrData = [ name, value ];

  if (idx < 0) {
    this.attrPush(attrData);
  } else {
    this.attrs[idx] = attrData;
  }
}
```
- example usage
```shell
...
} else {
  this.attrs = [ attrData ];
}
};


/**
 * Token.attrSet(name, value)
 *
 * Set 'name' attribute to 'value'. Override old value if exists.
 **/
Token.prototype.attrSet = function attrSet(name, value) {
var idx = this.attrIndex(name),
    attrData = [ name, value ];
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
