# Mensagens
```php
    <!-- Mensagem -->
    <script type="text/javascript">
    $(document).ready(function () {
    $('#success').click(function (e) {
      e.preventDefault()
      $('#message').html('<div class="alert alert-success fade in"><button type="button" class="close close-alert" data-dismiss="alert" aria-hidden="true">×</button>This is a success message</div>');
    })
    });
    </script>
    <div class="container">
    <h2>Buttons and Alerts</h2>
    <p class="lead">This example shows off how to use buttons and jQuery together. 
    Click the buttons to see the alert message. </p>
           <p>
           <form method="post">
            <button type="button" class="btn btn-success" id="success">Success</button>
         </form>
          </p>
          <div id="message"></div>
    </div>
```
