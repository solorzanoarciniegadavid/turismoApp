<script>

</script>

<div class="all-container">
    <div class="card">
        <div class="card-one">
            <img class="card-img" src="https://images.unsplash.com/photo-1591699396114-d936888e470f?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60" alt="Ephesus Picture">
            <h6 class="guided">Tour guiado</h6>
            <h2>Guanajuato</h2>
            <h5>Vamos a la ciudad del amor</h5>
        
            <div class="icon">
                <i class="fab fa-clock"> <span>Duración: 2 días </span></i><br>
                <i class="fa fa-running"> <span>Skip the line</span></i><br>
                <i class="fa fa-user-friends"> <span>Grupal </span></i>
            </div>
            <div class="prices">
                <span class="from">Desde</span>
                <span class="price"><i class="fa fa-usd"></i> 1,500</span>
                <span class="person">por persona</span>
            </div>
            <div>
              
            </div>
        </div>
    </div>
</div>



<style>

:root {
    --allday: #1593FF; /* h6 color */
    --guided: tomato; /* h6 color */
    --private: purple; /* h6 color */
    --daytrip: #d3de32; /* h6 color */
}
/* --------------------------------------------------------*/
/* Card Layout */
.card {
  overflow: hidden;
  background: white;
  box-shadow: 0 0 15px rgba(0, 0, 0, 0.2);
  height: 28rem;
  width: 30rem;
  margin: 3rem;
}

.card-img {
  height: 12rem;
  width: 30rem;
  object-fit: cover;
}

/* tittle style */
h2, h5, h6 {
  margin-left: 1rem;
}

h2 {
  font-weight: 600;
}

h5 {
  font-weight: 500;
  opacity: .9;
}
/* h2 style */
h2 {
  position: relative;
  top: -1em;
  font-size: 25px;
  font-weight: 700;
  letter-spacing: 1.1px;
}

h5 {
  position: relative;
  top: -2.7em;
  font-size: 16px;
  font-weight: 500;
  opacity: .8;
}
/* h6 style */
h6 {
  position: relative;
  display: inline;
  top: -1em;
  font-size: 15px;
  border-radius: 0.25em;
  padding: .2rem;
  color: white;
  font-weight: 500;
}

.allday {
  border: 1px solid var(--allday) ;
  background-color: var(--allday) ;
}

.guided {
  border: 1px solid var(--guided);
  background-color: var(--guided);
}

.daytrip {
  border: 1px solid var(--daytrip);
  background-color: var(--daytrip);
}

.private {
  border: 1px solid var(--private);
  background-color: var(--private);
}

/* Icon Style */
.icon {
  position: relative;
  top: -2.5em;
  right: -1em;
  font-family: 'Raleway', sans-serif;
  vertical-align: middle;
}

.fa-clock, .fa-running, .fa-user-friends {
  padding: 0.3rem;
  font-size: 1rem;
}

span {
  font-family: 'Raleway', sans-serif;
  font-weight: 500;
  font-size: .9rem;
  line-height: 1.2;
  opacity: .8;
}

/* Price Style */
.prices > .from {
  position: relative;
  top: -7em;
  right: -11.5em;
  font-size: 20px;
  opacity: .7;
}

.prices > .price {
  position: relative;
  top: -3.2em;
  right: -5.2em;
  font-size: 32px;
  opacity: .9;
}

.prices > .person {
  position: relative;
  top: -4.5em;
  right: -5.5em;
  font-size: 16px;
  opacity: .5;
}

/* Media Queries */
@media (min-width: 1499px) {
  /* For a screen > 1499px, this CSS will be read */
  .all-container {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-area: 20px;
    margin-left: 1rem;
  }
}
@media (min-width: 820px) and (max-width: 1499px) {
  /* For a screen > 820px, and < 1499 this CSS will be read */
  .all-container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-area: 20px;
    margin: auto 2rem;
  }
}
@media (max-width: 820px) {
  /* For a screen < 820px, this CSS will be read */
  .all-container {
    display: grid;
    grid-template-columns: 1fr;
    grid-area: 20px;
    margin: auto;
  }
}

</style>