.flip-card {
  background-color: transparent;
  width: 300px;
  height: 200px;
  perspective: 1000px;
}

/* This container is needed to position the front and back side */
.flip-card-inner {
  position: relative;
  width: 100%;
  height: 100%;
  text-align: center;
  transition: transform 1s ease;
  transform-style: preserve-3d;
}

.flip-card:hover .flip-card-inner {
  transform: rotateY(180deg);
}

/* Position the front and back side */
.flip-card-front, .flip-card-back {
  position: absolute;
  width: 100%;
  height: 100%;
  backface-visibility: hidden;
}

.flip-card-back img {
    width: 15rem;
}
.flip-card-back {
  width: 15rem;
  transform: rotateY(180deg);
}






    <main>
    <div class="container text-center">
  <div class="row row-cols-3 flip-card">
    <div class="col">
        <div class="flip-card-inner">
      <div class="card flip-card-front" style="width: 15rem">
        <img
          src="https://static-00.iconduck.com/assets.00/bomb-emoji-1959x2048-vuy7ly1m.png"
          class="card-img-top"
          alt="Bomb"
        />
      </div>
      <div class="flip-card-back">
        <img src="https://cdn.pixabay.com/photo/2013/04/01/21/30/fire-extinguisher-99147_1280.png" alt="Saved"/>
      </div>
        </div>
    </div>