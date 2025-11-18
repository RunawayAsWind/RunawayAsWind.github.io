# Comments
<!-- Markdown comments are invisible after rendering -->
&lt;!-- Comment here --&gt;
<br>
<br>
<br>
<br>

# Multi-line Breaks
You can use &lt;br&gt; for multiple line breaks
<br>
<br>
<br>
<br>

# Line Breaks
This is the first line. If you only press enter once and then write this line.
Then when rendered, these two lines will be tightly together, looking like the same paragraph.

But if you add a blank line between two sentences like this.

Then they will become two separate paragraphs with noticeable spacing.
<br>
<br>
<br>
<br>

# Horizontal Rule Syntax
First method***

***

Second method---

---

Third method___
___
<br>
<br>
<br>
<br>

# Heading Examples
# First Level Heading (H1)
## Second Level Heading (H2)
### Third Level Heading (H3)
#### Fourth Level Heading (H4)
##### Fifth Level Heading (H5)
###### Sixth Level Heading (H6)
<br>
<br>
<br>
<br>

# Paragraphs and Text Formatting
This is a normal paragraph. In Markdown, you just write text continuously. Paragraphs are separated by blank lines.

This is another paragraph.

**This is bold text**
__This is also bold text__

*This is italic text*
_This is also italic text_

***This is bold and italic text***
**_This is also bold and italic text_**

~~This is strikethrough text~~

`This is inline code` or ``This is also inline code``

<u>This is underlined text (non-standard, but some parsers support it)</u>
<br>
<br>
<br>
<br>

# Unordered List
- Item One
- Item Two
  - Nested Item Two Point One
  - Nested Item Two Point Two
    - Third Level Nesting
- Item Three

* Asterisks can also be used for unordered lists
+ Plus signs can also be used
<br>
<br>
<br>
<br>

# Ordered List
1. First Item
2. Second Item
   1. Nested First Item
   2. Nested Second Item
3. Third Item
<br>
<br>
<br>
<br>

# Task List
- [x] Completed task
- [ ] Incomplete task
- [ ] Another todo item
<br>
<br>
<br>
<br>

# Inline Links
[Go to OpenAI's official website](https://openai.com)
<br>
<br>
<br>
<br>

# Reference-style Links
This is an example of a reference-style link [OpenAI][1] and another example [Google][2].

[1]: https://openai.com
[2]: https://google.com "This is Google's tooltip text"
<br>
<br>
<br>
<br>

# Direct URLs
Visit https://github.com to check it out.
<br>
<br>
<br>
<br>

# Images
Web Image

<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub Logo" width="100" height="100">

Local Image

<img src="./Images/GitHub-Mark.png" alt="GitHub Logo" width="100" height="100">
<br>
<br>
<br>
<br>

# Tables
Simple Version

| Name | Age | City |
| :--- | :--: | ---: |
| Zhang San | 28 | Beijing |
| Li Si | 35 | Shanghai |
| Wang Wu | 22 | Guangzhou |
 
<br>
<br>

Merged Cells

<table>
  <tr>
    <th rowspan="2">Month</th>
    <th colspan="2">Sales Data</th>
  </tr>
  <tr>
    <th>Product A</th>
    <th>Product B</th>
  </tr>
  <tr>
    <td>January</td>
    <td>100</td>
    <td>150</td>
  </tr>
  <tr>
    <td>February</td>
    <td>80</td>
    <td>120</td>
  </tr>
</table>
<br>
<br>
<br>
<br>

# Code Blocks
C++

```cpp
// This is a simple C++ script
#include <iostream>
using namespace std;

int main() {
    cout << "Hello World!" << endl;
    return 0;
}
```
<br>
<br>

Python

```python
# This is a simple Python script
def main():
    print("Hello World!")

if __name__ == "__main__":
    main()
```
<br>
<br>

Bash
```bash
#!/bin/bash
# This is a simple Bash script
echo "Current directory: $(pwd)"
git status
```
<br>
<br>

Json
```json
{
  "name": "John Doe",
  "age": 30,
  "city": "New York",
  "hobbies": ["reading", "traveling"]
}
```
<br>
<br>
<br>
<br>

# Internal Navigation
Jumping within the same MD file
- [Comments](#comments)
- [Multi-line Breaks](#multi-line-breaks)
<br>
<br>

Jumping between different MD files
- [TestMD1](TestMD1)
- [TestMD2](TestMD2)
<br>
<br>
<br>
<br>

# Folding Box
<details>
<summary>Complete Documentation Directory</summary>

<div style="padding-left: 20px;">
  <details>
  <summary>User Documentation</summary>

  - [Document Example 1](TestMD1)

  </details>

  <details>
  <summary>Development Documentation</summary>

  - [Document Example 1](TestMD1)

      <details>
      <summary>User Documentation</summary>

      - [Document Example 1](TestMD1)

      </details>
  </details>

  <details>
  <summary>Development Documentation</summary>

  - [Document Example 1](TestMD1)

      <details>
      <summary>User Documentation</summary>

      - [Document Example 1](TestMD1)

      </details>
  </details>
</div>

</details>