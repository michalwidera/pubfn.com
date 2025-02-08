<!DOCTYPE html>
<html lang="en">

<head>

  {% include head.md %}

</head>

<body>

  <header class="masthead text-center">
    <div class="masthead-content">
      <div class="container">
        <h2 class="masthead-subheading"> {{ page.title }} </h2>
      </div>
    </div>
  </header>

  {% for item in site.sections %}
    <section>
      <div class="container">
        <div class="row align-items-center">
          {% if item.s1 and item.s1 != "" and item.s1 != nil %}
          <div class="{{ item.s1 }}">
            <div class="p-5">
              <img class="img-fluid rounded" src="{{ item.picture }}" alt="">
            </div>
          </div>
          {% endif %}
          <div class="{{ item.s2 }}">
            <div class="p-5">
              <h2 class="display-4">{{ item.name }}</h2>
              {{ item.content | markdownify }}
            </div>
          </div>
        </div>
      </div>
    </section>
  {% endfor %}

  {% include navigation.md %}
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

  <!-- Bootstrap core JavaScript -->
  <script src="vendor/jquery/jquery.min.js"></script>
  <script src="vendor/bootstrap/js/bootstrap.bundle.min.js"></script>

</body>

</html>
