<!-- Navigation -->
<nav class="navbar navbar-expand-lg navbar-dark navbar-custom fixed-top">
    <div class="container">
        <a class="navbar-brand" href="/">Pub fn</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarResponsive" aria-controls="navbarResponsive" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarResponsive">
        <ul class="navbar-nav ml-auto">
            {% for item in site.pages %}
            <li class="nav-item">
            <a class="nav-link" href="{{ item.permalink }}">{{ item.title }}</a>
            </li>
            {% endfor %}
        </ul>
        </div>
    </div>
</nav>