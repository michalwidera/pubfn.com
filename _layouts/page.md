<!DOCTYPE html>
<html lang="en">

<head>

  {% include head.md %}

</head>

<body>

  {% include navigation.md %}

  {{ content }}

  {% include footer.md %}

  <!-- Bootstrap core JavaScript -->
  <script src="{{ site.baseurl }}/vendor/jquery/jquery.min.js"></script>
  <script src="{{ site.baseurl }}/vendor/bootstrap/js/bootstrap.bundle.min.js"></script>

</body>

</html>
