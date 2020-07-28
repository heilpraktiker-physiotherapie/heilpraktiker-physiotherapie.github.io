---
layout: page
title: Anmeldeformular zur Fortbildung sektoraler Heilpraktiker Physiotherapie
metatitle: Führe hier Deine Anmeldung zur Fortbildung sektoraler Heilpraktiker Physiotherapie durch
description: Führe hier Deine Anmeldung zur Fortbildung sektoraler Heilpraktiker Physiotherapie durch
scssfile: 
customamp:
    - amp-mustache
---
<form class="sample-form" id="anmeldeform"
  method="post"
  action-xhr="https://prod-38.westeurope.logic.azure.com:443/workflows/4baba6ec8c34458cb30b3c2428be30c8/triggers/manual/paths/invoke?api-version=2016-06-01&sp=%2Ftriggers%2Fmanual%2Frun&sv=1.0&sig=XeRWzADA0FEO3ZDKmxH6_FJ_0tgyIC6ZNQLX2AOSLWc"
  target="_top">
  <input type="text"
    name="name"
    placeholder="Name..."
    required>
  <input type="email"
    name="email"
    placeholder="Email..."
    required>
  <input type="submit" id="submitButton"
    value="Subscribe">

  <div submit-success>
    <template type="amp-mustache">
      Success! Thanks {{name}} for trying the <code>amp-form</code> demo! Try to insert the word "error" as a name input in the form to see how <code>amp-form</code> handles errors.
    </template>
  </div>
  <div submit-error>
    <template type="amp-mustache">
      Error! Thanks {{name}} for trying the <code>amp-form</code> demo with an error response.
    </template>
  </div>
  <script>window.onload = function () {
    document.getElementById(“submitButton”).onclick = submitForm;
};
function submitForm()
{
   var formData = JSON.stringify($("anmeldeform").serializeArray());
   $.ajax({
  type: "POST",
  url: "serverUrl",
  data: formData,
  success: function(){},
  dataType: "json",
  contentType : "application/json"
});
}
</script>
</form>