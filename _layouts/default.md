<!DOCTYPE html>
<html lang="en">

<head>

  {% include head.md %}

</head>

<body>

  {% include navigation.md %}
  {% include header.md %}
  
  <header class="masthead text-center">
    <div class="masthead-content">
      <div class="container">
        <h2 class="masthead-subheading"> {{ page.title }} </h2>
      </div>
    </div>
  </header>

  <section>
    <div class="container">
      <div class="row align-items-center">
          <div class="col-lg-6 order-lg-1">
            <div class="p-5">
              {{ content }}
            </div>
          </div>
      </div>
    </div>
  </section>

  {% include footer.md %}

  <!-- Bootstrap core JavaScript -->
  <script src="vendor/jquery/jquery.min.js"></script>
  <script src="vendor/bootstrap/js/bootstrap.bundle.min.js"></script>

</body>

</html>
