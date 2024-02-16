# jQuery Tabs

Simply add tabs.

## Install

```bash
composer require agencenous/jquery-tabs
```

## Usage

```html
<style rel="stylesheet" href="/vendor/agencenous/jquery-tabs/jquery-tabs.css"/>
<script src="/vendor/agencenous/jquery-tabs/jquery-tabs.js"/>
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
- nextText,
- prevClass,
- nextClass

Full example

```javascript
jQuery('#form').createTabs({
		children: 'fieldset',
		childrenTitle: '.tab-title',
		hideUntilLast: 'input[type=submit]',
		prevText: '« back',
		nextText: 'Next »',
		prevClass: 'btn',
		nextClass: 'btn'
});
```

### Triggers

```javascript
jQuery('#form')
  .on('tab_ready', function(){
    console.log('READY!');
  })
  .on('tab_change', function(){
    console.log('TAB CHANGED!');
  })
.createTabs();
```
