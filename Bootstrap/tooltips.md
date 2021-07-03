# Tooltips

```php
    <!-- Tooltip -->
    <section>
    <div class="container">
        <a href="#" data-toggle="tooltip" data-placement="top" title="Top!">Hover</a>
        <a href="#" data-toggle="tooltip" data-placement="bottom" title="Bottom!">Hover</a>
        <a href="#" data-toggle="tooltip" data-placement="left" title="Left!">Hover</a>
        <a href="#" data-toggle="tooltip" data-placement="right" title="Right!">Hover</a>
    </div>
    </section>
    <script>
        $(document).ready(function () {
            $('[data-toggle="tooltip"]').tooltip();
        });
    </script>
```
