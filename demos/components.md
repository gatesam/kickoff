---
layout: demo
body-class: show-grid
navgroup: demo
navactive: democomponents
title: Components

meta:
  description: See Kickoff's components demo

next:
 - title: Typography demo
   body: See our default typography styles
   link: typography.html
 - title: Forms demo
   body: See how Kickoff handles forms
   link: forms.html
---
<a name="buttons"></a>

## Buttons
Button styles can be applied to anything with the `.btn` class applied. However, typically you'll want to apply these to only `<a>` and `<button>` elements for the best rendering.

#### Button sizes
Fancy larger or smaller buttons? Add `.btn--large`, or `.btn--small` for additional sizes. The colours used by this button are defined in our [colour palette](https://github.com/tmwagency/kickoff/blob/master/scss/_color-palette.scss#L38-L39) file.

<div class="demo">
	<div class="demo-visual">
		<h4>Normal size</h4>
		<a href="#" class="btn">Button</a>

		<h4>Large size</h4>
		<a href="#" class="btn btn--large">Default colour</a>

		<h4>Small size</h4>
		<a href="#" class="btn btn--small">Button</a>
	</div>

	<div class="demo-code">
{% highlight html%}
<!-- Normal buttons with default colour -->
<a href="#" class="btn">Button</a>

<!-- Larger buttons use the .btn--large modifier class -->
<a href="#" class="btn btn--large">Default colour</a>

<!-- Small buttons use the .btn--small modifier class -->
<a href="#" class="btn btn--small">Button</a>
{% endhighlight %}
	</div>
</div>

---

### Button styles
We provide only one button style variant because we think you should define your own. This variant, the *primary* button, uses the `.btn--primary` modifier class. We suggest setting up your own buttons in the same way, [see here](https://github.com/tmwagency/kickoff/blob/master/scss/partials/components/_buttons.scss#L81-L95).

The colours used by this button are defined in our [colour palette](https://github.com/tmwagency/kickoff/blob/master/scss/_color-palette.scss#L41-L42) file.

<div class="demo">
	<div class="demo-visual">
		<a href="#" class="btn btn--primary">Button</a>
	</div>

	<div class="demo-code">
{% highlight html%}
<!-- Add .btn--primary to use the primary colours -->
<a href="#" class="btn btn--primary">Button</a>
{% endhighlight %}
	</div>
</div>

---

### Block-level buttons
To make buttons span to 100% width, add the `.btn--block` modifier class. You can also see that we are using the `.btn--primary` modifier class as well as `.btn--block`.

<div class="demo">
	<div class="demo-visual">
		<a href="#" class="btn btn--block btn--primary">Button</a>
	</div>

	<div class="demo-code">
{% highlight html%}
<!-- Add .btn--block to use the block colours -->
<a href="#" class="btn btn--block btn--primary">Button</a>
{% endhighlight %}
	</div>
</div>

---

### Natural buttons
We have `.btn--natural` modifier class that inherits sizing from its parent. This is extremely useful when you have a button inside a paragraph or a heading.

<div class="demo">
	<div class="demo-visual">
		<p>
			With <code>.btn--natural</code> modifier class: <a href="#" class="btn btn--natural btn--primary">button</a>
		</p>
		<p>
			Without <code>.btn--natural</code> modifier class: <a href="#" class="btn btn--primary">button</a>
		</p>
	</div>
	<div class="demo-code">
{% highlight html%}
<a href="#" class="btn btn--natural btn--primary">With .btn--natural button</a>
{% endhighlight %}
	</div>
</div>

---

### Pill Buttons
Add the `.btn--pill` modifier class to any `.btn`.

<div class="demo">
	<div class="demo-visual">
		<p>
			<a href="#" class="btn btn--pill btn--primary">Primary pill</a>
			<a href="#" class="btn btn--pill">Default pill</a>
		</p>

		<!-- Add the .btn--natural modifier class to fix the padding -->
		<p>This is <a href="#" class="btn btn--primary btn--natural btn--pill"> a button </a> in a paragraph!</p>
	</div>
	<div class="demo-code">
{% highlight html%}
<!-- Pill buttons use the .btn--pill modifier class -->
<a href="#" class="btn btn--pill btn--primary">Pill</a>
<a href="#" class="btn btn--pill">This is a Pill</a>

<p>This is <a href="#" class="btn btn--primary btn--natural btn--pill"> a button </a> in a paragraph!</p>
{% endhighlight %}
	</div>
</div>

---

<a name="mediaobject"></a>

## Media Object
Place any image- and text-like content side-by-side, as per: [media object](http://stubbornella.org/content/2010/06/25/the-media-object-saves-hundreds-of-lines-of-code)

<div class="demo">
	<div class="demo-visual">
		<div class="media">
			<div class="media-img">
				<img src="http://hhhhold.com/s">
			</div>
			<div class="media-body">
				<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
			</div>
		</div>
		<div class="media media--rev">
			<div class="media-body">
				<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
			</div>
			<div class="media-img">
				<img src="http://hhhhold.com/m">
			</div>
		</div>
	</div>
	<div class="demo-code">
{% highlight html%}
<!-- Media element with left aligned image -->
<div class="media">
	<div class="media-img">
		<img src="http://hhhhold.com/s">
	</div>
	<div class="media-body">
		<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
	</div>
</div>

<!-- Media element with right aligned image -->
<div class="media media--rev">
	<div class="media-body">
		<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
	</div>
	<div class="media-img">
		<img src="hhhhold.com/m">
	</div>
</div>
{% endhighlight %}
	</div>
</div>

---

<a name="fluidvideo"></a>

## Fluid video
<div class="demo">
	<div class="demo-visual">
		<div class="fluidVideo">
			<iframe width="560" height="315" src="//www.youtube-nocookie.com/embed/CjB_oVeq8Lo" frameborder="0" allowfullscreen></iframe>
		</div>
	</div>
	<div class="demo-code">
{% highlight html%}
<div class="fluidVideo">
	<iframe width="560" height="315" src="//www.youtube-nocookie.com/embed/CjB_oVeq8Lo" frameborder="0" allowfullscreen></iframe>
</div>
{% endhighlight %}
	</div>
</div>

---

<a name="blockgrids"></a>

## Block grids
<div class="demo">
	<div class="demo-visual">
		<ul class="l-blockGrid l-blockGrid--4up l-blockGrid--2up--narrow">
			<li>Item 1</li>
			<li>Item 2</li>
			<li>Item 3</li>
			<li>Item 4</li>
			<li>Item 5</li>
			<li>Item 6</li>
			<li>Item 7</li>
			<li>Item 8</li>
		</ul>
	</div>
	<div class="demo-code">
{% highlight html%}
<ul class="l-blockGrid l-blockGrid--4up l-blockGrid--2up--narrow">
	<li>Item 1</li>
	<li>Item 2</li>
	<li>Item 3</li>
	<li>Item 4</li>
</ul>
{% endhighlight %}
	</div>
</div>

---

<a name="lists"></a>

## Lists
<div class="demo">
	<div class="demo-visual">
		<h4>Centre-aligned lists</h4>
		<ul class="l-list--centred">
			<li>Item 1</li>
			<li>Item 2</li>
			<li>Item 3</li>
			<li>Item 4</li>
		</ul>
		<h4>Floated lists</h4>
		<ul class="l-list--floated">
			<li>Item 1</li>
			<li>Item 2</li>
			<li>Item 3</li>
			<li>Item 4</li>
		</ul>
	</div>
	<div class="demo-code">
{% highlight html%}
<!-- Centre-aligned lists -->
<ul class="l-list--centred">
	<li>Item 1</li>
	<li>Item 2</li>
	<li>Item 3</li>
	<li>Item 4</li>
</ul>

<!-- Floated lists -->
<ul class="l-list--floated">
	<li>Item 1</li>
	<li>Item 2</li>
	<li>Item 3</li>
	<li>Item 4</li>
</ul>
{% endhighlight %}
	</div>
</div>

---

<a name="tables"></a>

## Tables
<div class="demo">
	<div class="demo-visual">
		<table class="table table--bordered table--striped table--hover table--rounded" cellpadding="0" cellspacing="0">
			<thead>
				<th>Table head</th>
				<th>Table head</th>
				<th>Table head</th>
			</thead>
			<tbody>
				<tr>
					<td>Table cell</td>
					<td>Table cell</td>
					<td>Table cell</td>
				</tr>
				<tr>
					<td>Table cell</td>
					<td>Table cell</td>
					<td>Table cell</td>
				</tr>
			</tbody>
			<tfoot>
				<td>Table foot</td>
				<td>Table foot</td>
				<td>Table foot</td>
			</tfoot>
		</table>
	</div>
	<div class="demo-code">
{% highlight html%}
<table class="table table--bordered table--striped table--hover table--rounded" cellpadding="0" cellspacing="0">
	<thead>
		<th>Table head</th>
		<th>Table head</th>
		<th>Table head</th>
	</thead>
	<tbody>
		<tr>
			<td>Table cell</td>
			<td>Table cell</td>
			<td>Table cell</td>
		</tr>
	</tbody>
	<tfoot>
		<td>Table foot</td>
		<td>Table foot</td>
		<td>Table foot</td>
	</tfoot>
</table>
{% endhighlight %}
	</div>
</div>

---

<a name="rwdtables"></a>
## Responsive tables
<div class="demo">
	<div class="demo-visual">
		<div class="tableResponsive">
			<table class="table" cellpadding="0" cellspacing="0">
				<thead>
					<th>Table Cell</th>
					<th>Table Cell</th>
					<th>Table Cell</th>
					<th>Table Cell</th>
					<th>Table Cell</th>
				</thead>
				<tbody>
					<tr>
						<td>Table Cell</td>
						<td>Table Cell</td>
						<td>Table Cell</td>
						<td>Table Cell</td>
						<td>Table Cell</td>
					</tr>
					<tr>
						<td>Table Cell</td>
						<td>Table Cell</td>
						<td>Table Cell</td>
						<td>Table Cell</td>
						<td>Table Cell</td>
					</tr>
					<tr>
						<td>Table Cell</td>
						<td>Table Cell</td>
						<td>Table Cell</td>
						<td>Table Cell</td>
						<td>Table Cell</td>
					</tr>
				</tbody>
				<tfoot>
					<td>Table Cell</td>
					<td>Table Cell</td>
					<td>Table Cell</td>
					<td>Table Cell</td>
					<td>Table Cell</td>
				</tfoot>
			</table>
		</div>
	</div>
	<div class="demo-code">
{% highlight html%}
<div class="tableResponsive">
	<table class="table" cellpadding="0" cellspacing="0">
		<thead>
			<th>Table Cell</th>
			<th>Table Cell</th>
			<th>Table Cell</th>
			<th>Table Cell</th>
			<th>Table Cell</th>
		</thead>
		<tbody>
			<tr>
				<td>Table Cell</td>
				<td>Table Cell</td>
				<td>Table Cell</td>
				<td>Table Cell</td>
				<td>Table Cell</td>
			</tr>
		</tbody>
		<tfoot>
			<td>Table Cell</td>
			<td>Table Cell</td>
			<td>Table Cell</td>
			<td>Table Cell</td>
			<td>Table Cell</td>
		</tfoot>
	</table>
</div>

{% endhighlight %}
	</div>
</div>

---

<a name="tabs"></a>

## Tabs
<div class="demo">
	<div class="demo-visual">
		<!-- Default, left-aligned tabs -->
		<ul class="tabs">
			<li><a href="#tabs-example-1" class="is-active">Tab 1</a></li>
			<li><a href="#tabs-example-2">Tab 2</a></li>
		</ul>
		<!-- Centre-aligned tabs -->
		<ul class="tabs tabs--alignCenter">
			<li><a href="#tabs-example-1" class="is-active">Tab 1</a></li>
			<li><a href="#tabs-example-2">Tab 2</a></li>
		</ul>
		<!-- Right-aligned tabs -->
		<ul class="tabs tabs--alignRight">
			<li><a href="#tabs-example-1" class="is-active">Tab 1</a></li>
			<li><a href="#tabs-example-2">Tab 2</a></li>
		</ul>
	</div>
	<div class="demo-code">
{% highlight html%}
<!-- Default, left-aligned tabs -->
<ul class="tabs">
	<li><a href="#tabs-example-1" class="is-active">Tab 1</a></li>
	<li><a href="#tabs-example-2">Tab 2</a></li>
</ul>

<!-- Centre-aligned tabs -->
<ul class="tabs tabs--alignCenter">
	<li><a href="#tabs-example-1" class="is-active">Tab 1</a></li>
	<li><a href="#tabs-example-2">Tab 2</a></li>
</ul>

<!-- Right-aligned tabs -->
<ul class="tabs tabs--alignRight">
	<li><a href="#tabs-example-1" class="is-active">Tab 1</a></li>
	<li><a href="#tabs-example-2">Tab 2</a></li>
</ul>
{% endhighlight %}
	</div>
</div>
