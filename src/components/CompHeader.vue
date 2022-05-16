<template>
  <div class="nome text-center">
    <h1>SITEFLIX</h1>
  </div>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid">
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarScroll"
        aria-controls="navbarScroll"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarScroll">
        <ul
          class="navbar-nav me-auto my-2 my-lg-0 navbar-nav-scroll"
          style="--bs-scroll-height: 100px"
        >
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Início</a>
          </li>
             <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Filmes</a>
          </li>
             <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Séries</a>
          </li>
             <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Doramas</a>
            
          </li>
        </ul>
        <form class="d-flex">
          <input
            class="form-control me-2"
            type="search"
            placeholder="Search"
            aria-label="Search"
          />
          <button class="btn btn-outline-success" type="submit">Search</button>
        </form>
      </div>
    </div>
  </nav>
  <div id="carouselExampleControls" class="carousel slide" data-ride="carousel">
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img
          id="aven"
          class="d-block w-100"
          src="./imgs/torre.jpg"
          alt="Primeiro Slide"
        />
      </div>
      <div class="carousel-item">
        <img
          class="d-block w-100"
          src="./imgs/attack.jpeg"
          alt="Segundo Slide"
        />
      </div>
    </div>
    <a
      class="carousel-control-prev"
      href="#carouselExampleControls"
      role="button"
      data-slide="prev"
    >
    </a>
    <a
      class="carousel-control-next"
      href="#carouselExampleControls"
      role="button"
      data-slide="next"
    >
    </a>
  </div>
</template>
