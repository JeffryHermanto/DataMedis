<template>
<div class="welcome">
  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <a class="navbar-item" href="#">
        <img src="../assets/logo-datamedis-header.png" alt="Bulma: a modern CSS framework based on Flexbox">
      </a>

      <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false">
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
      </a>
    </div>
  </nav>

  <div class="container">

    <!-- HEMATOLOGI -->
    <div class="box">
      <div class="content">
        <p><i class="fas fa-angle-down"></i> &nbsp;Hematologi</p>
      </div>
      <div class="columns">
        <div class="column is-one-fifth">
          <div class="tooltip">
            LED
            <span class="tooltiptext">
              <strong>Laju Endap Darah</strong> <br />
              <em>Erythrocyte sedimentation rate (ESR)</em> adalah kecepatan sel - sel darah merah mengendap di dalam tabung uji dengan satuan mm/jam.<br />
              <a href="https://id.wikipedia.org/wiki/Laju_endap_darah" target="_blank"><small><em><u>Klik untuk melihat halaman Wikipedia terkait</u></em></small></a>
            </span>
          </div>
        </div>
        <div class="column is-four-fifth">
          <progress class="progress is-primary is-large" value="75" max="100">75%</progress>
        </div>
      </div>
    </div>

    <!-- IMUNOSEROLOGI -->
    <div class="box">
      <div class="content">
        <p><i class="fas fa-angle-down"></i> &nbsp;Imunoserologi</p>
      </div>
      <div class="columns">
        <div class="column is-one-fifth">
          <p>Protein Spesifik</p>
        </div>
        <div class="column is-four-fifth">
          <progress class="progress is-danger is-large" value="45" max="100">45%</progress>
          <div class="flag tooltip">
            <i class="fas fa-comment-alt"></i>
            <span class="tooltipGraph">
              <img src="../assets/CRPKuantitatif.jpg" />
            </span>
          </div>
        </div>
      </div>
    </div>

  </div>
</div>
</template>

<script>
export default {
  name: 'Welcome'
}
</script>

<style>
.container {
  margin-top: 60px
}

.tooltip {
  position: relative;
  display: inline-block;
}

.tooltip .tooltiptext {
  visibility: hidden;
  width: 320px;
  background-color: #f0fafc;
  color: #1c696b;
  text-align: left;
  border-radius: 6px;
  border: 1px solid #1c696b;
  padding: 15px;

  /* Position the tooltip */
  position: absolute;
  z-index: 1;
  top: 100%;
}

.tooltip:hover .tooltiptext {
  visibility: visible;
}

.flag {
  position: relative;
  z-index: 1;
  top: -62px;
  left: 25%;
  font-size: 1.2em;
  color: orange
}

.tooltip .tooltipGraph {
  visibility: hidden;
  width: 320px;
  background-color: #f0fafc;
  color: #1c696b;
  text-align: center;
  border-radius: 6px;
  border: 1px solid #1c696b;
  padding: 2px;

  /* Position the tooltip */
  position: absolute;
  z-index: 1;
  top: 100%;
}

.tooltip:hover .tooltipGraph {
  visibility: visible;
}
</style>
