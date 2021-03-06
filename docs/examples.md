---
layout: examples
title: Examples
permalink: /examples/
stylesheet: '//!site.cdn!/!site.version!/quill.snow.css'
---

# Examples

The two examples below demonstrate what is possible with Quill. Check out how they interact with each other!

## Basic Example

A basic editor with just a few formats to get started.

<div class="quill-wrapper">
  <div id="basic-toolbar" class="toolbar">
    <select title="Size" class="ql-size">
      <option value="10px">Small</option>
      <option value="13px" selected>Normal</option>
      <option value="18px">Large</option>
      <option value="32px">Huge</option>
    </select>
    <button class="ql-bold">Bold</button>
    <button class="ql-italic">Italic</button>
  </div>
  <div id="basic-editor" class="editor">
  {% include lotr.html %}
  </div>
</div>

<a class="accordian-toggle" data-toggle="collapse" href="#basic-collapse">Show/Hide Code</a>

<div id="basic-collapse" class="accordian-body collapse">
{% highlight javascript %}
{% include basic-editor.html %}
{% endhighlight %}
</div>

## Full Example

Uses all the features of Quill, including [Modules](/docs/modules/) and [Themes](/docs/themes/).

<div class="quill-wrapper">
  <div id="full-toolbar" class="toolbar">
    {% include full-toolbar.html %}
    <span class="ql-format-group">
      <span title="Link" class="ql-format-button ql-link"></span>
    </span>
  </div>
  <div id="full-editor" class="editor">
  {% include lotr.html %}
  </div>
</div>

<a class="accordian-toggle" data-toggle="collapse" href="#full-collapse">Show/Hide Code</a>

<div id="full-collapse" class="accordian-body collapse">
{% highlight javascript %}
{% include full-editor.html %}
{% endhighlight %}
</div>

<script src="//{{site.cdn}}/{{site.version}}/quill.js"></script>
<script>
{% include basic-editor.html %}
{% include full-editor.html %}
</script>
