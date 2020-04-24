# jQuery Tabs

Simply add tabs.

## Usage

```html
<style rel="stylesheet" href="jquery-tabs/jquery-tabs.css"/>
<script" src="jquery-tabs/jquery-tabs.js"/>
```

## Example

```html
<div class="content">
  <section>
    <h3>Section 1</h3>
    <p>Somme content</p>
  </section>
  <section>
    <h3>Section 2</h3>
    <p>Somme content</p>
  </section>
  <section>
    <h3>Section 3</h3>
    <p>Somme content</p>
</section>
</div>
```

And then, just instanciate:

```javascript
jQuery('.content').createTabs({
		children: 'section',
		childrenTitle: 'h3'
});
```

### Additional params

- hideUntilLast
- prevText,
- nextText

Full example

```javascript
jQuery('#form').createTabs({
		children: 'fieldset',
		childrenTitle: '.tab-title',
		hideUntilLast: 'input[type=submit]',
		prevText: '« back',
		nextText: 'Next »'
});
```
