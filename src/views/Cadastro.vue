<template>
  <div>
    <h1>Cadastro de Usuarios</h1>

    <div class="container">
      <!-- Stack the columns on mobile by making one full-width and the other half-width -->
      <div class="row">
        <div class="g-col-md-8">.col-md-8</div>
        <div class="p-3 border bg-light">Custom column padding</div>
        <div class="col-6 col-md-4">.col-6 .col-md-4</div>
        <div class="p-3 border bg-light">Custom column padding</div>
      </div>

      <!-- Columns start at 50% wide on mobile and bump up to 33.3% wide on desktop -->
      <div class="row">
        <div class="col-6 col-md-4">.col-6 .col-md-4</div>
        <div class="col-6 col-md-4">.col-6 .col-md-4</div>
        <div class="col-6 col-md-4">.col-6 .col-md-4</div>
      </div>

      <!-- Columns are always 50% wide, on mobile and desktop -->
      <div class="grid">
        <div class="g-col-6">.col-6</div>
        <div class="g-col-6">.col-6</div>
      </div>
    </div>

    <div class="container">
      <div class="row row-cols-4">
        <div class="col">Column</div>
        <div class="col">Column</div>
        <div class="col">Column</div>
        <div class="col">Column</div>
      </div>
    </div>

    <div class="container">
      <div class="row row-cols-1 row-cols-sm-2 row-cols-lg-4">
        <div class="col">Column</div>
        <div class="col">Column</div>
        <div class="col">Column</div>
        <div class="col">Column</div>
      </div>
    </div>

    <div class="container">
      <div class="row">
        <div class="col align-self-start">One of three columns</div>
        <div class="col align-self-center">One of three columns</div>
        <div class="col align-self-end">One of three columns</div>
      </div>
    </div>

    <div class="container px-4">
      <div class="row gx-5">
        <div class="col">
          <div class="p-3 border bg-light">Custom column padding</div>
        </div>
        <div class="col">
          <div class="p-3 border bg-light">Custom column padding</div>
        </div>
      </div>
    </div>
  </div>
</template>
