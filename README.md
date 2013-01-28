#What does it do?

This plugin replaces the default checkboxes and radio inputs for better looking ones. 
Check the [landing page](http://arthurgouveia.com/prettyCheckable/) for a demo.

##Features:

* Compatible with IE7+, Chrome, Firefox, Safari and mobile browsers;
* Automatic Labee Detection, which will help you implment structed programming
* Better look & size;
* Super easy implementation;
* Selectable with Tab and checkable with keyboard;
* Change events & Chainning preserved;
* More area of click/touch. A plus for mobile devices.

##Install & Setup

    <link rel="stylesheet" href="js/prettyCheckable/prettyCheckable.css">

    <script src="js/prettyCheckable/prettyCheckable.js"></script>

Write your inputs and add a class for the jQuery selector:

    <input type="checkbox" class="myClass" value="yes" id="answer" name="answer"/>

Setup prettyCheckable for your inputs and you're all set:

    $().ready(function(){

      $('input.js-pretty-select').prettyCheckable();

    });

You can start the plugin with the options you see on the documentation bellow and they will be applied to all matching inputs:

    $().ready(function(){

      $('input.js-pretty-select').prettyCheckable({
        color: 'red'
      });

    });

If you want to apply something to all the inputs but you need a few specific ones to be different, you can add the specifics inline:

    <input type="checkbox" class="myClass" value="yes" id="answer" name="answer" data-color="green" />

##Documentation

###Label Association
<pre>
	<div class="input checkbox">
		<input type="checkbox" id="PropertyIsActive" value="1" name="data[Property][is_active]">
		<label for="PropertyIsActive">Active?</label>
	</div>
</pre>

In this scenario the Label Active? will be automagically added to Pretty checkbox. This will let you write code which will work smooth even without js

*None of the parameters is mandatory.*

###Options

<table>
  <tbody>
    <tr>
      <td>Name</td>
      <td>Values</td>
      <td>Description</td>
    </tr>
    <tr>
      <td>
        <strong>labelPosition</strong>
      </td>
      <td>
        string<br>
        <em>left, right(default)</em>
      </td>
      <td>
        <p>This is the position where the label for the inputs should be placed, if informed.</p>
      </td>
    </tr>
    <tr>
      <td>
        <strong>customClass</strong>
      </td>
      <td>
        string<br>
        <em>A class name.</em>
      </td>
      <td>
        <p>This will add a class you want to the wrapping div surrounding the input, created by the plugin.</p>
      </td>
    </tr>
    <tr>
      <td>
        <strong>color</strong>
      </td>
      <td>
        string<br>
        <em>blue(default), green, yellow or red</em>
      </td>
      <td>
        <p>Choose between one of the four colors options.</p>
      </td>
    </tr>
  </tbody>
</table>

###Inline Options

*All inline configs will overwrite the ones you initialized the plugin with.*

<table class="table table-striped">
  <tbody>
    <tr>
      <td>Name</td>
      <td>Values</td>
      <td>Description</td>
    </tr>
    <tr>
      <td>
        <strong>data-label</strong>
      </td>
      <td>
        string<br>
        <em>Text for your label</em>
      </td>
      <td>
        <p>If informed, this will create a label attached to the input.</p>
      </td>
    </tr>
    <tr>
      <td>
        <strong>data-labelPosition</strong>
      </td>
      <td>
        string<br>
        <em>left, right(default)</em>
      </td>
      <td>
        <p>This is the position where the label for the inputs should be placed, if informed.</p>
      </td>
    </tr>
    <tr>
      <td>
        <strong>data-customClass</strong>
      </td>
      <td>
        string<br>
        <em>A class name.</em>
      </td>
      <td>
        <p>This will add a class you want to the wrapping div surrounding the input, created by the plugin.</p>
      </td>
    </tr>
    <tr>
      <td>
        <strong>data-color</strong>
      </td>
      <td>
        string<br>
        <em>blue(default), green, yellow or red</em>
      </td>
      <td>
        <p>Choose between one of the four colors options.</p>
      </td>
    </tr>
  </tbody>
</table>


###Support

* Reach me at http://subin.me