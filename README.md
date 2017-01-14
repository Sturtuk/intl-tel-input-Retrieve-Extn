# intl-tel-input-Retrieve-Extn
jQuery Script for getting intl-tel-input Extn Without Utils Script


```html
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/intl-tel-input/10.0.6/css/intlTelInput.css" />
<script src="https://cdnjs.cloudflare.com/ajax/libs/intl-tel-input/10.0.6/js/intlTelInput.min.js"></script>
<script>
  jQuery(document).ready(function($){
	   $.noConflict();

             $("#phone").intlTelInput({
  
                autoPlaceholder: true,
                preferredCountries: ['in', 'us', 'gb']
            });
 });
 </script>

 

        <form action="" method="post"  >
                  <input type="hidden" name="Cextn" id="Cextn" />
                  <input type="text" id="phone" name="phone" class="input-text" value=""  maxlength="13"/>
                  <input type="submit" name="submit"  value="submit" />
        </form>
 ```
 
 **To Retrieve the Extn of the Phone Number**
 ```js
 <script>
  var data = $('.selected-flag').attr('title');
  $("#Cextn").val(data);
</script>
```
