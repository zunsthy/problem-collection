# Devtools Network Panel decode `FormData` incorrectly

## Introduction

Decode FormData payload with wrong encoding in devtools network panel.

## Issues

Firefox: [Bugzilaa](https://bugzilla.mozilla.org/show_bug.cgi?id=2034306)

## Reproduce

Create a form with file. Select file and fill some name or field with CJK charactors. Submit it.

Or open [the page](https://zunsthy.github.io/problem-collection/devtools-network-panel-decode-incorrect-for-formdata) to try.

Firefox:

![file name error](pics/d-file-name.jpg)

![text name and value error](pics/d-input-name-value.jpg)

If submit data has no file, encoding recognition is correct.

![no file](pics/no-file.jpg)
