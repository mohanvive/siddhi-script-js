# API Docs - v5.0.1

## Script

### javascript *<a target="_blank" href="https://siddhi.io/en/v5.0/docs/query-guide/#script">(Script)</a>*

<p style="word-wrap: break-word">This extension allows you to include JavaScript functions within the Siddhi Query Language.</p>

<span id="syntax" class="md-typeset" style="display: block; font-weight: bold;">Syntax</span>
```
define function <FunctionName>[javascript] return <type> {
    // Script code
};
```

<span id="examples" class="md-typeset" style="display: block; font-weight: bold;">Examples</span>
<span id="example-1" class="md-typeset" style="display: block; color: rgba(0, 0, 0, 0.54); font-size: 12.8px; font-weight: bold;">EXAMPLE 1</span>
```
define function concatJ[JavaScript] return string {"  var str1 = data[0];
 var str2 = data[1];
 var str3 = data[2];
 var res = str1.concat(str2,str3);
 return res;
};
```
<p style="word-wrap: break-word">This JS function will consume 3 var variables, concatenate them and will return as a string</p>

